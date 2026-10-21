# ㈜위드프레쉬 QC 일지

HACCP 일지를 휴대폰·태블릿 브라우저로 작성하고, PC에서 조회·결재·인쇄하는 웹페이지입니다.
기록은 Firebase Realtime Database(`withfresh-haccp`)에 저장됩니다.

## 주소 (휴대폰·태블릿)

| 페이지 | 주소 | 용도 |
|---|---|---|
| 메뉴 (첫 화면) | https://jindori1204-pixel.github.io/qc-logs/ | 모든 일지로 이동 |
| 조회·결재 | https://jindori1204-pixel.github.io/qc-logs/review.html | 전체 일지 조회·결재·인쇄 (13개 탭) |
| 온도 점검 일지 | https://jindori1204-pixel.github.io/qc-logs/temperature_log.html | 냉장·냉동고 온도 (1일 3회) |
| 일반위생관리 점검표 | https://jindori1204-pixel.github.io/qc-logs/hygiene_log.html | 일일·주간·월간·분기·연간 위생점검 |
| 방충·방서 점검표 | https://jindori1204-pixel.github.io/qc-logs/pest_log.html | 포충등·트랩 점검 |
| 폐기물 반출대장 | https://jindori1204-pixel.github.io/qc-logs/waste_log.html | 폐기물 반출·처리업체 |
| 공정관리 점검일지 | https://jindori1204-pixel.github.io/qc-logs/process_log.html | 제품군별 공정 점검 (CCP 포함) |
| 원재료 육안검사 | https://jindori1204-pixel.github.io/qc-logs/material_log.html | 원료 입고 검사·품온 사진 |
| 부자재 육안검사 | https://jindori1204-pixel.github.io/qc-logs/submaterial_log.html | 포장재 등 입고 검사 |
| 개인위생 점검표 | https://jindori1204-pixel.github.io/qc-logs/personal_hygiene_log.html | 작업자 개인위생 |
| 운송차량 점검표 | https://jindori1204-pixel.github.io/qc-logs/vehicle_log.html | 입고·출고 차량 |
| CCP 검증점검표 | https://jindori1204-pixel.github.io/qc-logs/ccp_log.html | 금속검출·소독·세척 CCP 검증 |
| 원료입고 | https://jindori1204-pixel.github.io/qc-logs/incoming_log.html | 원료 입고 기록 |
| MF 산지직송 검품일지 | https://jindori1204-pixel.github.io/qc-logs/mf_inspection_log.html | MF 출고품 검품 (검품기준서 WF-QC-104) |

공정관리 점검일지는 [📋 생산일보에서 불러오기]를 누르면 그날 생산한 제품군 목록이 나오고, 제품군을 누르면 양식·제품명·LOT·원료 LOT이 채워집니다. 적/부와 측정값은 점검 후 직접 입력합니다. 주소 끝에 `?date=2026-10-21`을 붙이면 그 날짜로 열립니다.

MF 검품일지는 주소 끝에 `?date=2026-10-21` 처럼 날짜를 붙이면 그 날짜의 작성 대기 기록을 바로 불러옵니다.

## 홈 화면에 추가

- **아이폰 (Safari)**: 메뉴 주소 접속 → 아래쪽 공유 버튼 → **홈 화면에 추가**
- **갤럭시 (Chrome)**: 메뉴 주소 접속 → 오른쪽 위 ⋮ → **홈 화면에 추가**

## 예전 화면이 보일 때

브라우저 캐시 때문입니다. 주소 뒤에 `?v=숫자`를 붙여 다시 여세요.
예: `https://jindori1204-pixel.github.io/qc-logs/review.html?v=5` (숫자는 아무거나, 바꿀 때마다 새로 받음)

## 데이터 원칙

- 점검 결과(○/×, 측정값)는 현장 점검자가 실제로 점검한 뒤 직접 입력합니다. 스크립트로 일괄 입력하지 않습니다.
- MF 검품일지의 "작성 대기" 기록에는 생산·물류일보(쿠팡 수불대장) 기준 품목·출고수량·LOT만 들어 있습니다.
