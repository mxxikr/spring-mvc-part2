김영한님의 [스프링 MVC 2편 - 백엔드 웹 개발 활용 기술](https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81-mvc-2/dashboard) 실습 코드 아카이브

---

### 💻 Development Environment

* Java 21
* Spring Boot 4.0.1
* Gradle
* IDE: IntelliJ

### 🏆 실습 목표

* 타임리프(Thymeleaf)의 기본 기능부터 스프링 통합, 폼 처리까지 서버 사이드 렌더링 기술 습득
* 메시지, 국제화, 검증(Validation) 등 실제 웹 애플리케이션에 필수적인 기능 구현
* 로그인(쿠키/세션)과 보안(필터/인터셉터) 로직을 단계별로 고도화하며 웹 보안의 원리 이해
* API 예외 처리, 타입 컨버터, 파일 업로드 등 스프링의 심화 기능 학습

### 📝 Curriculum

1. [**타임리프 - 기본 기능**](https://mxxikr.github.io/posts/thymeleaf-basic-features/)
    * 텍스트(`text`, `utext`), SpringEL, 기본 객체 및 유틸리티 객체 활용
    * 연산, 조건부 평가, 반복, 블록(`th:block`), 자바스크립트 인라인 등 문법 실습
    * 템플릿 조각(Fragment)과 레이아웃 상속을 통한 화면 모듈화


2. [**타임리프 - 스프링 통합과 폼**](https://mxxikr.github.io/posts/spring-mvc-thymeleaf-spring-integration/)
    * `th:object`, `th:field`를 이용한 스프링 폼 데이터 처리 및 통합
    * 체크 박스(단일/멀티), 라디오 버튼, 셀렉트 박스 등 다양한 폼 요소 핸들링


3. [**메시지, 국제화**](https://mxxikr.github.io/posts/spring-mvc-message-internationalization/)
    * 스프링 메시지 소스(`MessageSource`) 설정 및 관리 방법
    * 웹 애플리케이션 국제화(i18n) 적용 및 브라우저 언어 설정 테스트


4. [**검증1 - Validation**](https://mxxikr.github.io/posts/spring-mvc-validation/)
    * `Map`을 이용한 직접 검증 한계 분석 및 `BindingResult` 스프링 통합
    * `FieldError`, `ObjectError` 처리와 `MessageCodesResolver` 메시지 관리 전략
    * 검증 로직을 `Validator` 인터페이스로 분리하여 체계적으로 관리


5. [**검증2 - Bean Validation**](https://mxxikr.github.io/posts/spring-mvc-bean-validation/)
    * 애노테이션 기반 검증(`@NotNull`, `@NotBlank`) 적용 및 `groups` 기능 활용
    * `MethodArgumentNotValidException` 예외 처리 및 `@RequestBody` JSON 데이터 검증


6. [**로그인 처리1 - 쿠키, 세션**](https://mxxikr.github.io/posts/spring-mvc-login-session/)
    * 영속/세션 쿠키의 생성과 보안 문제점(위변조, 도용) 이해
    * 세션의 동작 원리 및 서블릿 `HttpSession`을 활용한 로그인 구현


7. [**로그인 처리2 - 필터, 인터셉터**](https://mxxikr.github.io/posts/spring-mvc-filter-interceptor/)
    * 서블릿 필터(Filter)를 활용한 공통 관심사(요청 로그, 인증) 해결
    * 스프링 인터셉터(Interceptor)의 호출 흐름 이해 및 필터와의 차이점 비교
    * `ArgumentResolver`를 활용한 `@Login` 커스텀 애노테이션 구현


8. [**예외 처리와 오류 페이지**](https://mxxikr.github.io/posts/spring-mvc-exception-handling/)
    * 서블릿 예외(`sendError`) 발생 시 컨테이너 동작과 필터/인터셉터의 흐름(`DispatcherType`)
    * 스프링 부트 `BasicErrorController`를 활용한 HTML/API 오류 페이지 일원화


9. [**API 예외 처리**](https://mxxikr.github.io/posts/spring-mvc-api-exception-handling/)
    * `HandlerExceptionResolver`(`ResponseStatus`, `DefaultHandler`)의 이해
    * `@ExceptionHandler`와 `@ControllerAdvice`를 활용한 실무형 전역 예외 처리


10. [**스프링 타입 컨버터**]()
    * `Converter`, `Formatter` 인터페이스 이해 및 커스텀 컨버터 구현
    * `ConversionService`를 통한 타입 변환의 일원화 및 뷰 템플릿 적용


11. [**파일 업로드**]()
    * `multipart/form-data` 전송 방식의 이해
    * 서블릿 `Part`와 스프링 `MultipartFile`을 이용한 파일 저장 및 다운로드 기능 구현
