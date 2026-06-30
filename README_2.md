# 데이터 안내

이 프로젝트의 원본 데이터는 홈랩(Proxmox + pfSense + Suricata)에서 실시간으로 수집한 IDS 경보 로그(`alerts.log`)입니다.

- **기간**: 2026-06-01 ~ 2026-06-29 (28일)
- **건수**: 약 82,918건
- **형식**: Suricata fast.log 포맷 (`[**] [sid] 시그니처설명 [**] [Classification: ...] [Priority: N] {PROTO} src_ip:port -> dst_ip:port`)

용량 및 운영 환경 보안상 이유로 원본 로그는 레포에 포함하지 않았습니다.

샘플 데이터를 받으려면 노트북 상단의 다운로드 셀을 실행하세요 (Google Drive 공유 링크에서 `gdown`으로 받아옵니다).

직접 재현하려면 동일한 정규식 파서로 자신의 Suricata `fast.log`를 파싱하면 됩니다 (`notebooks/analysis.ipynb`의 2~3절 참고).
