
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

## Team

Isaak Alemu: voice and face models, accuracy evaluation, AI analysis layer.