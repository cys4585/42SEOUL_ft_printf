# 2. ft_printf

`ft_putnbr()`, `ft_putstr()`로는 충분하지 않으니까

# Summary

이 프로젝트의 목표는 꽤 간단하다. `printf()`를 재코딩한다. 가변인자를 사용하는 방법에 대해 배우게 된다. 얼마나 멋져? 사실 꽤 멋져 :)

---

# Introduction

인기 있고 다재다능한 C 함수인 `printf()`를 발견하게 될 것이다. 이 연습은 프로그래밍 기술을 향상시킬 수 있는 좋은 기회이다. 보통 정도의 난이도이다.

C에서 변수 함수(variadic functions)를 발견하게 될 것이다. 성공적인 `ft_printf`의 핵심은 잘 구조화되고 확장 가능한 코드이다.

**(Information) 이 과제가 통과되면, `libft`에 너의 `ft_printf()`를 추가할 수 있을 것이고, 그러므로 그것을 학교의 C 프로젝트에 사용할 수 있을 것이다.**

---

# Mandatory part

| Program name | libftprintf.a |
| --- | --- |
| Turn in files | Makefile, *.h, */*.h, *.c, */*.c |
| Makefile | NAME, all, clean, fclean, re |
| External functs. | malloc, free, write, va_start, va_arg, va_copy, va_end |
| Libft authorized | Yes |
| Description | 원본 printf()와 유사한 함수인 ft_printf()가 포함된 라이브러리 작성 |

libc의 printf() 함수를 재코딩해야 한다.

- 프로토타입: `int ft_printf(const char *, ...);`
- 요구사항
    - 원본 printf()의 버퍼 관리를 구현하지 마라.
    - 함수에서 다음 변환을 처리해야 한다. `cspdiuxX%`
    - 너의 함수는 원본 `printf()`와 비교될 것이다.
    - 라이브러리를 만들려면 명령어 `ar`를 사용해야 한다. `libtool` 명령 사용은 금지된다.
    - `libftprintf.a`는 저장소의 루트에 생성되어야 한다.
    - 다음 변환을 구현해야 합니다.
        - `%c`: 단일 문자를 인쇄
        - `%s`: 일반 C 규칙에 정의된 대로 문자열을 인쇄
        - `%p`: `void *` 포인터 인수는 16진수 형식으로 인쇄
        - `%d`: 십진수(밑수 10)를 인쇄
        - `%i`: 밑이 10인 정수를 인쇄
        - `%u`: 부호 없는 십진수(밑 10) 숫자를 인쇄
        - `%x`: 16진수(밑 16) 소문자 형식으로 숫자를 인쇄
        - `%X`: 16진수(베이스 16) 대문자 형식으로 숫자를 인쇄
        - `%%` 백분율 기호(%)를 인쇄

---

# Submission and peer-evaluation

평소처럼 Git 저장소에 과제를 제출해라. 방어 중에는 리포지토리 내부의 작업만 평가된다. 파일이 정확한지 확인하기 위해 파일 이름을 다시 확인해라.

이 과제가 통과되면,  `libft`에 `ft_printf()`를 추가할 수 있을 것이고, 그러므로 그것을 학교의 C 프로젝트에 사용할 수 있을 것이다.

---

# 참고

[C 언어 코딩 도장](https://dojang.io/mod/page/view.php?id=577)