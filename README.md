# java-lotto-precourse

# 📋 기능 목록 - 1차

---

## 💵 로또 발매기 프로그램

### 주요 기능

- [ ]  자동 로또 발행
- [ ]  수동 로또 당첨번호 생성
- [ ]  로또 수익률 계산

### 유효성 검증

- [ ]  ‘**로또 구입 금액**’은 숫자 이외의 값이어서는 안 된다.
- [ ]  ‘**로또 구입 금액**’이 너무 클 수 없다 (정수 오버플로가 발생해선 안 된다.)
- [ ]  ‘**로또 구입 금액**’은 1,000원 단위로 나누어떨어져야 한다. (즉, 1000으로 나눈 나머지가 0이어야 한다.)
- [ ]  ‘**로또번호**’는 1~45로 구성되어있어야 한다.
- [ ]  ‘**로또의 로또 번호 개수는**’는 6이어야만 한다.

---

# MVC

# **[Model]**

### 1. Lotto - 로또

- 자동 로또 번호 발행
- 유효성 검증
    - 로또 번호가 6개인지 확인
    - 로또가 1~45로 구성되었는지 확인

### 2. WinningLotto - 당첨 로또 번호

- 당첨 로또 번호 생성
- 유효성 검증
    - 로또 번호가 6개인지 확인
    - 로또가 1~45로 구성되었는지 확인

### 3. WinningResult - 당첨금액 및 수익률

- 당첨금액 계산 로직
- 수익률 계산 로직
- 유효성 검증

# [View]

## InputView

### 1. LottoTicketPrice - 로또 티켓 가격 입력

### 2. WinningNumber - 당첨 번호 입력 뷰

### 3. BonusNumber - 보너스 번호 입력 뷰

## OutputView

### ResultView

### 1. LottoTicketView - 발행한 로또 수량 및 번호 출력 뷰

### 2. WinningResultView - 당첨 내역 출력 뷰

### 3. RateOfReturnView - 수익률 출력 뷰

### ExceptionView - 예외 상황 시 에러 문구 출력 뷰 [ERROR] + 에러메시지

# [Controller]

### 1. LottoController - 로또 발행부터 수익률 출력까지의 흐름 제어