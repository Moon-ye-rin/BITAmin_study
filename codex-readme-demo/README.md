# BITAmin

## 1. 프로젝트 개요

이 프로젝트는 파이썬으로 만든 간단한 계산기 예제입니다.  
`src/calculator.py`에 사칙연산 함수가 있고, `src/main.py`에서 이 함수를 불러 실행 결과를 출력합니다.  
기초적인 함수 작성, 모듈 분리, 프로그램 실행 방법을 연습하기에 적합한 구조입니다.

## 2. 폴더 구조

```text
BITAmin/
├─ src/
│  ├─ __init__.py
│  ├─ calculator.py
│  └─ main.py
├─ tests/
│  ├─ __init__.py
│  └─ test_calculator.py
├─ AGENTS.md
├─ README.md
└─ requirements.txt
```

## 3. 설치 방법

1. 저장소 폴더로 이동합니다.
2. 필요한 패키지를 설치합니다.

```bash
pip install -r requirements.txt
```

## 4. 실행 방법

이 프로그램은 `src/main.py`를 실행하면 동작합니다.

```bash
python -m src.main
```

실행하면 덧셈, 뺄셈, 곱셈, 나눗셈 결과가 화면에 출력됩니다.

## 5. 테스트 방법

테스트는 `pytest`로 실행할 수 있습니다.

```bash
pytest
```

현재 `tests/test_calculator.py` 파일은 비어 있으므로, 실행 시 테스트가 0개로 표시됩니다.  
즉, 테스트 실행 명령은 준비되어 있지만 실제 테스트 코드는 아직 작성되지 않은 상태입니다.

## 6. 주요 함수 설명

### `src/calculator.py`

- `add(a, b)`  
  두 수 `a`와 `b`를 더한 값을 반환합니다.

- `subtract(a, b)`  
  첫 번째 수에서 두 번째 수를 뺀 값을 반환합니다.

- `multiply(a, b)`  
  두 수를 곱한 값을 반환합니다.

- `divide(a, b)`  
  첫 번째 수를 두 번째 수로 나눈 값을 반환합니다.  
  단, 두 번째 수가 `0`이면 나눌 수 없으므로 `ValueError`를 발생시킵니다.

### `src/main.py`

- `main()`  
  계산기 함수들을 불러와 예시 숫자로 계산을 수행하고 결과를 출력합니다.  
  프로그램을 직접 실행하면 이 함수가 호출됩니다.
