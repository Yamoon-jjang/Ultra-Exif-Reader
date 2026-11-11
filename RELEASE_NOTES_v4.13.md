# Ultra Exif Reader v4.13

이미지·영상의 카메라 EXIF 및 AI 생성 메타데이터를 분석하는 브라우저용 단일 HTML 도구입니다.

### 🇰🇷 이번 업데이트
- **MiniMax H3 Chain 영상 지원:** 여러 장면을 이어 만든 H3 Chain 영상의 실행 기록(`h3_manifest`)을 읽어 장면별 **실제 프롬프트·Seed·Steps·생성/최종 프레임**을 표시합니다. 프롬프트는 기록에 저장된 SHA-256 해시로 원문 여부를 검증합니다.
- 공통 프롬프트와 장면별 프롬프트를 원문 그대로 구분해 표시하고, 계획에만 있는 장면은 실행 결과로 표시하지 않습니다.
- 계획 전체 프레임과 실제 영상 프레임, 장면별 생성·최종 프레임을 구분합니다.
- 2^53을 넘는 큰 Seed도 끝자리까지 정확히 표시합니다.
- 영상의 prompt JSON에 `NaN` 값이 있으면 prompt 전체가 버려져 모델·Seed·Steps가 틀리게 나오던 문제를 고쳤습니다. 정상 JSON은 기존과 똑같이 읽습니다.
- 실행 기록이 없거나 손상된 H3 Chain 파일은 쓰이지 않은 옛 위젯 값 대신 "확인 불가"로 표시합니다.
- H3 Chain 기록이나 `NaN` 값이 없는 파일은 v4.12와 동일하게 표시됩니다.

### 🇺🇸 English
- **MiniMax H3 Chain videos:** Reads the execution record (`h3_manifest`) of multi-scene H3 Chain videos and shows each executed scene's real prompt (SHA-256 verified), Seed, Steps and generated/final frame counts.
- Shows the common prompt and each scene prompt exactly as recorded; planned-only scenes are never shown as results.
- Seeds above 2^53 are shown exactly.
- Video prompt JSON containing `NaN` tokens is no longer discarded, so model/Seed/Steps match the equivalent PNG result. Valid JSON is read exactly as before.
- H3 Chain files without a usable execution record show "unavailable" instead of stale widget values.
- Files without H3 Chain records or `NaN` tokens are shown exactly as in v4.12.

### 사용 방법 / Installation
1. **Assets**에서 `Ultra_exif_reader_v4.13.zip`을 다운로드해 압축 해제합니다.
2. Chrome 또는 Edge에서 `Ultra_exif_reader_v4.13.html`을 엽니다.
3. 이미지·영상·ZIP 파일을 불러와 메타데이터를 확인합니다.

기본 메타데이터 확인은 별도 프로그램 설치 없이 가능하며, 이미지 AI 분석 및 번역 등 일부 기능은 외부 서비스·API 설정이 필요할 수 있습니다.

*Note: Some media do not contain generation metadata; missing fields are not fabricated.*
