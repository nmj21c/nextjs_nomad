# Next.js

## - URL 라우팅
1. app > page.tsx 파일들 알아서 라우팅 해줌 

    - app/page.tsx = localhost:3000/
    - app/test/page.tsx = localhost:3000/test

2. 404 not found = app > not-found.tsx 

## - "use client" Directive

1. 이 Directive 가 있어도 server side 에서 미처리 되는건 아님
2. 아마도 client 에서도 뭔가 interective(상호작용) 있는 경우 선언
3. use client 가 있어야 hydrate 됨
4. 없으면 SSR에서 넘어온 html 그대로 유지됨

## - Link tag

1. Server side rendering 된 상태에서는 a 태그 와 같음 MAP 동작
2. Client side rendering (hydration) 된 이후엔 reflesh 없이 SPA 로 동작

    ex)
    ```
    <Link href="/">Root</Link>
    ```

## Hydration

1. SSR -> CSR 변환 작업