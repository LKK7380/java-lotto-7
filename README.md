# 기능 명세서

## 1. 로또 구입 기능
### InputView
- [x] 구입 금액 입력
  - [x] "구입금액을 입력해 주세요." 안내 문구 출력
  - [x] 입력값이 숫자가 아닐 경우 예외 처리
  - [x] 0원 이하일때 예외 처리
  - [x] 1,000원 단위가 아닐 경우 예외 처리
### OutputView
- [x] 구매한 로또 수량 출력
  - [x] "n개를 구매했습니다." 형식으로 출력
- [x] 발행된 로또 번호들 출력
  - [x] "[1, 2, 3, 4, 5, 6]" 형식으로 출력
## 2. 로또 번호 생성 기능
### Lotto
- [x] 로또 번호 자동 생성
  - [x] 6개의 숫자만 가능
  - [x] 중복된 숫자 불가능
  - [x] 1~45 사이의 숫자만 가능
  - [x] 오름차순 정렬하여 저장

## 3. 당첨 번호 입력 기능
### InputView
- [ ] 당첨 번호 6개 입력
  - [ ] "당첨 번호를 입력해 주세요." 안내 문구 출력
  - [x] 6개의 숫자 검증
  - [x] 쉼표(,)로 구분하여 입력
  - [x] 1~45 사이의 숫자만 가능
  - [x] 중복된 숫자 불가능
- [ ] 보너스 번호 1개 입력
  - [ ] "보너스 번호를 입력해 주세요." 안내 문구 출력
  - [x] 1~45 사이의 숫자만 가능
  - [x] 당첨 번호와 중복 불가능

## 4. 당첨 확인 기능
### LottoResult
- [x] 구매한 로또와 당첨 번호 비교
- [x] 당첨 등수 확인
  - [x] 1등: 6개 번호 일치
  - [x] 2등: 5개 번호 + 보너스 번호 일치
  - [x] 3등: 5개 번호 일치
  - [x] 4등: 4개 번호 일치
  - [x] 5등: 3개 번호 일치
### LottoPrize
- [x] 당첨금 확인
  - [x] 1등: 2,000,000,000원
  - [x] 2등: 30,000,000원
  - [x] 3등: 1,500,000원
  - [x] 4등: 50,000원
  - [x] 5등: 5,000원

## 5. 당첨 결과 출력 기능
### OutputView
- [x] 당첨 내역 출력
  - [x] "당첨 통계" 헤더 출력
  - [x] "---" 구분선 출력
  - [x] 각 등수별 당첨 내역 출력
- [x] 수익률 계산 및 출력
  - [x] 소수점 둘째 자리에서 반올림
  - [x] 수익률은 퍼센트로 출력