# Humoyun Turaev (Ray)

Full-stack and DevOps engineer based in Incheon, Korea. I lead web development on the
Medical Software R&D team at Seeann Solution. We build an ordering platform for doctors,
an internal office platform, and the servers both of them run on.

I've been working since 2020, first remotely for European product teams and now in Korea.
I speak Korean, English, Russian and Uzbek.

Portfolio: https://h1turaev.github.io\
Resume: [Korean](https://h1turaev.github.io/files/resume-ko.pdf), [English](https://h1turaev.github.io/files/resume-en.pdf)\
Email: tuhucu97@gmail.com

## Recent work

- The legacy servers had 1,800+ PM2 restarts. I grouped the logs by cause and fixed them one at a time. In the five days after the fix there were zero.
- The list API went from 291 to 966 rps after adding 304 responses and caching. Repeat-visit TTFB dropped from 82 to 32 ms.
- Peak memory in AI segmentation went from 1.68 GiB to 122 MiB. I traced it to a single allocation and processed it in chunks. The output is identical.
- Per-app database pools went from up to 1,000 connections down to 50. The MySQL limit is 151.
- SSL for 15 hostnames now renews automatically.

The details and how each one works are on the portfolio.

## Right now

I'm rolling out a monitoring agent on our AWS and Windows GPU servers. It watches PM2,
Docker, NGINX, SSL certificates and database connections. Rules handle the failures we
already know: restart a process, reload NGINX, renew a certificate. An LLM helps sort out
the rest. After every action it checks again and sends one summary to Telegram. Anything
outside the allowed actions goes to a person.

Outside work I'm building Point2Point, a taxi service for Uzbekistan, and Milli, a
national messenger for Uzbekistan.

## Stack

- Frontend: Next.js, React, TypeScript, React Native (Expo), Three.js, vtk.js
- Backend: Node.js, NestJS, Express, Fastify, Python (FastAPI), REST, GraphQL, Socket.IO
- Data: MySQL, PostgreSQL, MongoDB, Redis, ScyllaDB, Prisma, Kysely
- Infrastructure: AWS (EC2, S3), Docker, NGINX, PM2, Terraform, GitHub Actions, GitLab CI, Prometheus, Grafana, Linux
- AI: RAG, MCP, LLM tool calling, GPU job queues

I'm open to remote freelance and contract work, in Korea or abroad. Email is the fastest way to reach me.
