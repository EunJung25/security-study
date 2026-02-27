2026-02-27

SameSite 종류

SameSite = None
-모든 요청에 쿠키 전송
-CSRF 방어 안 됨
(요즘은 None 쓰면 Secure 필수)

SameSite = Lax
-일반적인 링크 클릭은 쿠키 전송
-POST 같은 상태 변경 요청에는 쿠키 안 보냄

(대부분 CSRF공격 차단 가능)

SameSite = Strict
-같은 사이트에서 온 요청만 쿠키 전송
-외부에서 들어오면 쿠키 안 보냄

(가장 강력하지만 UX 불편할 수 있음)


