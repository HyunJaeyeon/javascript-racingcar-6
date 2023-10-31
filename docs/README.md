# 2주차 - 🚘 자동차 경주

- [2주차 - 🚘 자동차 경주](#2주차----자동차-경주)
  - [🔍 기능 요구 사항](#-기능-요구-사항)
  - [🔍 입력 예외 처리](#-입력-예외-처리)
  - [🗂️ 구현할 기능 목록](#️-구현할-기능-목록)
  - [💡 더 생각해보기](#-더-생각해보기)

## 🔍 기능 요구 사항

1. **게임 실행**
2. **자동차 이름 입력**
   - 각 이름은 5자 이하로
   - 쉼표 기준으로 자동차 이름 구분
3. **시도할 횟수 입력**
4. **전진 / 멈춤 판단**
   - 0~9 랜덤값 구하기
   - 값에 따라 전진/멈춤 여부 결정
     - 값이 4~9이면, 전진
     - 값이 0~3이면, 정지
5. **게임 실행 결과 출력**
   - `{자동차 이름} : --` 형태로 출력
   - `시도 횟수` 순서대로 전부 출력
6. **최종 우승자 출력**
   - 자동차들의 `이동거리값` 비교
     - 최대값 가진 자동차이름 출력 (1대 이상)

---

## 🔍 입력 예외 처리

`[ERROR]`로 시작하는 메시지 `throw`

- **자동차 이름 입력**
  - 이름 입력값이 없는 경우
  - 이름이 5자를 넘는 경우
  - ,가 양끝에 (불필요한 ,가)있는 경우
- **시도할 횟수 입력**
  - 0을 입력한 경우 (0은 게임시작이 아니라고 판단)
  - 숫자가 아닐 경우

---

## 🗂️ 구현할 기능 목록

`[Model]`

- [x] 자동차 이름 입력
  - [ ] 쉼표 기준 이름 구분
  - [ ] 공백 제거
  - [ ] 자동차와 이동거리값 객체 생성
  - [ ] 입력값 객체에 저장
- [x] 시도할 횟수 입력

`[View]`

- [ ] 게임 실행 결과 출력 형태 설정
- [ ] 최종 우승자 출력 형태 설정

`[Controller]`

- [ ] 0~9 랜덤값 따라 전진/멈춤 여부 결정
- [ ] `시도`차수별 결과 출력
- [ ] 거리 이동만큼 각 객체에 넣기
- [ ] 자동차들의 `이동거리값` 비교
- [ ] 우승자 선정
- [ ] 게임 실행

`[Exception]`

- [ ] 자동차 이름 입력 예외처리
- [ ] 시도할 횟수 예외처리

`[Test]`

- [ ] 테스트 코드 작성

---

## 💡 더 생각해보기

- 테스트코드 작성법
- 에러 throw