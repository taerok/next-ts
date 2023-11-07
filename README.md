# 프로젝트 설정

이 프로젝트는 pre-commit과 git-conventional-commit을 사용하여 일관된 코드 스타일과 커밋 메시지 규칙을 유지합니다.

## pre-commit 설정 방법

1. 먼저, pre-commit을 설치하려면 다음 명령을 실행해야 합니다:

   ```sh
   pip install pre-commit
   ```

2. pre-commit hook을 설치하려면 프로젝트 루트에서 다음 명령을 실행하세요:

   ```sh
   pre-commit install
   ```

이제 커밋을 하기 전에 정의된 pre-commit hook이 실행됩니다.

## git-conventional-commit 사용하기

커밋 메시지는 git-conventional-commit 규칙을 따라야 합니다. 이를 자동화하기 위해 다음 단계를 따르세요:

1. 각 커밋 메시지는 다음 형식을 따라야 합니다:

    <pre>
    <b><a href="https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13#types">&lt;type&gt;</a></b>(<b><a href="https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13#scopes">&lt;optional scope&gt;</a></b>): <b><a href="https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13#description">&lt;description&gt;</a></b>
    <sub>empty separator line</sub>
    <b><a href="https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13#body">&lt;optional body&gt;</a></b>
    <sub>empty separator line</sub>
    <b><a href="https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13#footer">&lt;optional footer&gt;</a></b>
    </pre>

   여기서 `type`은 변경 사항의 유형(예: `feat`, `fix`, `docs`, `style` 등)을 나타내고, `description`은 간단한 설명입니다.

2. 커밋을 하기 전에 `.pre-commit-config.yaml` 파일에 정의된 훅이 커밋 메시지를 검증합니다.


## Getting Started

First, run the development server:

```bash
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
