# Ultra Exif Reader v4.12

이미지·영상의 카메라 EXIF 및 AI 생성 메타데이터를 분석하는 브라우저용 단일 HTML 도구입니다.

### 🇰🇷 이번 업데이트
- **실제 생성 프롬프트 표시:** Ultra Qwen Image Editor + PiD(v1.0.4 이상)와 Ultra Image + PiD(v1.0.2 이상)가 이미지에 기록한 실제 입력 프롬프트(`ultra_generation_prompts`)를 읽어 **Positive / Final CLIP**에 표시합니다.
- 번역기·LLM 노드를 거친 프롬프트도 번역 후 실제 문장이 표시되고, 변환 전 원문은 **Original / Source**에 함께 표시됩니다.
- Image Saver(Simple)로 저장한 PNG·JPEG·WebP를 모두 지원합니다.
- 기록이 없는 기존 이미지는 v4.11과 동일하게 표시됩니다.

### 🇺🇸 English
- Reads the executed prompt record (`ultra_generation_prompts`) written by Ultra Qwen Image Editor + PiD v1.0.4+ and Ultra Image + PiD v1.0.2+, and shows it as **Positive / Final CLIP**.
- Prompts passed through translator or LLM nodes now show the real converted text, with the original text kept as **Original / Source**.
- Supports PNG, JPEG and WebP saved by Image Saver (Simple).
- Images without the record are shown exactly as in v4.11.

### 사용 방법 / Installation
1. **Assets**에서 `Ultra_exif_reader_v4.12.zip`을 다운로드해 압축 해제합니다.
2. Chrome 또는 Edge에서 `Ultra_exif_reader_v4.12.html`을 엽니다.
3. 이미지·영상·ZIP 파일을 불러와 메타데이터를 확인합니다.

기본 메타데이터 확인은 별도 프로그램 설치 없이 가능하며, 이미지 AI 분석 및 번역 등 일부 기능은 외부 서비스·API 설정이 필요할 수 있습니다.

*Note: Some media do not contain generation metadata; missing fields are not fabricated.*
