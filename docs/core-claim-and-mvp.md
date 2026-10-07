# Core claim and MVP

## Core claim

QorannooDhugaa will show that matching a respondent's voice and face can catch duplicate and fake survey submissions at a measured accuracy, without storing names, phone numbers or ID numbers with the answers. It will also show that an interface that reads every question aloud alongside the text lets respondents complete a survey by listening, without needing to read.

Accuracy is measured on public datasets (used within their licenses) and synthetic data.

## Founders

- **Surra Bulto:** product, backend, offline-first app, security, deployment, documentation and commercial work.
- **Isak Alemu:** voice and face models, accuracy evaluation and the AI analysis layer.

## Supporting benefits

- Cost and time saved compared with paper surveys, such as travel time to remote communities and the number of paper forms carried.
- Reliable offline collection: answers are saved on the phone and sent later, so remote places with weak internet can still be reached.

These are measured when a study with real users is approved (see Testing).

## Background

Many communities take a long day of travel to reach, and paper-based research means carrying large numbers of forms. Fraud and duplicate entries are hard to detect, and text-heavy surveys leave out people who cannot read. These are the problems this project is built for.

## Who uses it

**Customers** are organizations or individuals who run digital research in Africa: universities, NGOs, churches and other faith-based institutions, and individual researchers.

Within one survey, three kinds of people use the app:

- **Researcher:** designs the survey and reads the results. Needs trustworthy data and a simple way to build and manage surveys.
- **Enumerator:** takes the survey to respondents in the field. Needs a fast, simple tool, and is also the person the system must be able to check.
- **Respondent:** answers the questions. Needs to understand each question, feel safe, and answer privately.

**Privacy rule:** the respondent answers privately and the enumerator never sees the answers. Respondents use their own phone when they have one. Otherwise the enumerator lends a phone, steps away from the screen, and the respondent uses earphones.

## Testing

During development, the founders test only with their own data, with close friends who have agreed in writing (a message is enough), with public datasets used within their license, and with synthetic data. Friends' data is deleted when testing ends.

Some volunteers use the app in a voice-only condition (text hidden) to check whether a survey can be completed without reading. Results from this informal testing are used internally and are not published as claims.

**Limitation:** volunteers who can read, using voice-only, show that the interface works without reading. They do not prove that people who cannot read will succeed. A publishable study with real respondents needs ethics approval and a legal review first, and is planned after the first release.

## Languages

Afaan Oromoo, Amharic and English. All three languages get the same features. The founders and volunteer friends speak all three, so translations and recordings can be checked in-house.

## How respondents answer

One interface serves everyone. Every question shows text and plays voice at the same time. The respondent can stop the voice and read, or keep listening.

- **Closed questions** (yes/no, choose one): the question and options are read aloud, and the respondent taps a large button or picture.
- **Open-ended questions:** the respondent can type or record a spoken answer. The recording is saved as the answer.
- **Transcription:** every spoken answer is saved as a recording and also transcribed automatically, in all three languages (Afaan Oromoo, Amharic and English), using speech-to-text models whose licenses allow commercial use. The original recording is always kept, and the transcript is a suggestion that the researcher can read, listen against and correct. Accuracy is measured separately for each language on public datasets and reported openly. Transcripts that fall below an agreed accuracy level are marked "low confidence" instead of being hidden. Another African language can be added after the first release, once the process works for these three.
## Out of scope for the first version

- A native mobile app and fingerprint matching. The first version is a web app; a mobile app may follow after publication, based on customer feedback.
- Languages beyond the three above. Another African language may be added after the first release.
- White-label branding and multiple survey templates. One sample template is enough.
- A separate mode for people who cannot read. The single interface above serves everyone.
- Hosting or operating the platform for other organizations.