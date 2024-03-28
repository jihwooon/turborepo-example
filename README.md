# Turborepo starter
Turborepo와 pnpm을 활용한 모노레포로 구성되어 있습니다.

## Tech Stack
- Nest.js
- Next.js
- TypeScript

## Getting Started
- Repository 복제합니다.
- `pnpm install` 을 실행하여 dependencies 항목 설치합니다.
- `pnpm run dev`로 프로젝트를 실행합니다.

## Run Started
Nestjs와 Nextjs를 동시에 실행 명령어는 다음과 같습니다.
```bash
pnpm dev
```
독립적으로 Nestjs 실행 명령어는 다음과 같습니다.
```bash
cd apps/web
pnpm run dev
```
독립적으로 Nestjs 실행 명령어는 다음과 같습니다.
```bash
cd apps/api
pnpm run start
pnpm run dev # watch mode
```

## Deploy Setting
프로젝트를 배포 전 빌드를 수행해야 합니다.

본 프로젝트는 TurboRepo로 배포를 수행합니다.
```bash
pnpm run build
```
이후 Docker-Compose로 Docker 배포를 수행합니다.
```bash
docker-compose build -d
```
