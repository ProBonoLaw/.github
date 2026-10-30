# ProBono Law

**Legal tooling for people who can't afford a lawyer.**

The code isn't here yet. This page explains what's coming, and why it's worth the wait.

## What this is

ProBono Law is a working production system, built to give self-represented litigants a
real chance in court. It:

- drafts the **declarations** you actually file
- turns a pile of evidence into an indexed, referenced **exhibit list**
- reconstructs a **timeline** out of your own documents
- answers **questions against your case record**
- runs an **argument builder** that constructs the opposing side's case against you, so
  you find your weak points before opposing counsel does

It ingests documents, audio and video, so a hearing recording becomes searchable evidence.

## Why it isn't public yet

It has been running as private infrastructure wired into a live Azure environment, and the
repositories still carry the identifiers and configuration that come with that. Publishing
them as they stand would be careless.

Before anything lands here, each repository is being:

1. scrubbed of environment identifiers and internal configuration
2. licensed under **Apache-2.0**
3. moved into this organization

Better to take the extra weeks and release something a clinic can actually deploy.

## Who it's for

**Legal aid clinics and self-help centers** — it will be yours to run. Free, no license
fee, and without needing to talk to anyone first.

**Developers** — there will be work worth doing.

No signup, no waitlist. When it's up, it's up.

---

*Built because the cost and complexity of being heard is where most people stop.*
