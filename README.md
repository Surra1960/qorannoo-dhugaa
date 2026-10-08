
# QorannooDhugaa

[![CI](https://github.com/Surra1960/qorannoo-dhugaa/actions/workflows/ci.yml/badge.svg)](https://github.com/Surra1960/qorannoo-dhugaa/actions/workflows/ci.yml)

## What is QorannooDhugaa?

QorannooDhugaa is an open-source research platform for collecting survey data in the field across Africa. It uses voice and face matching to detect duplicate or fraudulent submissions, without storing names or ID numbers with survey answers. It also gives non-literate respondents an audio-first interface in their own language.

## The problem it solves

- **Field fraud:** enumerators may fabricate or duplicate survey responses.
- **Privacy vs. verification:** proving a respondent is a unique person usually means collecting identifying details, which discourages honest answers on sensitive topics.
- **Language and literacy exclusion:** text-heavy forms leave out non-literate and rural respondents.
- **Slow qualitative analysis:** open-ended answers take weeks to transcribe and code by hand.

## Project status

In development, Phase 0.

## Planned features

- Multi-tenant platform with database-level data isolation
- Audio-first, pictorial survey interface with configurable local languages
- Survey builder and XLSForm import
- Offline-first Progressive Web App with automatic sync
- Dual-biometric (voice + face) duplicate detection
- Pseudonymous participant tokens that separate identity from responses
- Assisted theme analysis of open-ended answers

## How to self-host

Coming soon.

## Run the database

The project uses PostgreSQL with the pgvector extension, run by Docker Compose. You need [Docker Desktop](https://www.docker.com/products/docker-desktop/) running.

1. Copy the example settings and set your own password in `.env` (this file is git-ignored and must never be committed):

```
   copy .env.example .env
```

   On macOS or Linux use `cp .env.example .env`.

2. Start the database:

```
   docker compose up -d
```

3. Check that it works. The status should say `healthy`:

```
   docker compose ps
```

   Then check that the `vector` extension is installed (Windows cmd):

```
   docker compose exec db sh -c "psql -U $POSTGRES_USER -d $POSTGRES_DB -c 'SELECT extname, extversion FROM pg_extension;'"
```

   On macOS or Linux, swap the quotes: use single quotes around the `sh -c` part and double quotes inside it.

4. Stop (data is kept):

```
   docker compose down
```

5. Reset (deletes all database data):

```
   docker compose down -v
```

The database listens on `127.0.0.1:15432` only, so it is not reachable from the network. To connect with a tool such as pgAdmin, use host `127.0.0.1`, port `15432`, and the user, password and database name from your `.env`.

## Team

Isaak Alemu: voice and face models, accuracy evaluation, AI analysis layer.