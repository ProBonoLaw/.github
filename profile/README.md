# ProBono Law

**Legal tooling for people who can't afford a lawyer.**

The code is here. All of it, under Apache-2.0.

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

## The code

| Repository | What it does | Stack |
|---|---|---|
| [pbl-ui](https://github.com/ProBonoLaw/pbl-ui) | Web UI and API | TypeScript |
| [pbl-file-operations](https://github.com/ProBonoLaw/pbl-file-operations) | Document and website ingestion, transformation, indexing, evidence extraction | TypeScript |
| [PBL-AIMIE-Service](https://github.com/ProBonoLaw/PBL-AIMIE-Service) | AI moderation and intuitive engagement | Python |
| [PBL-AIMIE-Operations](https://github.com/ProBonoLaw/PBL-AIMIE-Operations) | Document generation workers, Markdown converter | C# |
| [PBL-Account-Operations](https://github.com/ProBonoLaw/PBL-Account-Operations) | Account services and tests | C# |
| [PBL-Email-Operations](https://github.com/ProBonoLaw/PBL-Email-Operations) | Email workers and notification clients | C# |
| [pbl-infrastructure](https://github.com/ProBonoLaw/pbl-infrastructure) | Pulumi infrastructure for the whole platform | TypeScript |

Every repository was scrubbed of environment identifiers and internal configuration
before it landed here. If you find something that slipped through, open an issue and say
so plainly — that's a bug, and it gets fixed the same day.

## Running it yourself

Every repository documents its own build and configuration. Start with
[pbl-infrastructure](https://github.com/ProBonoLaw/pbl-infrastructure) — it stands up the
platform on Azure with Pulumi, and its **Deploying from a private copy** section is
written for exactly this: taking the public source and running it as your own.

From there, each service carries what it needs — requirements, local configuration,
testing, and rollout. The platform assumes Azure. Moving it elsewhere is real work, and
if you do it, the rest of us would like the patch.

## Who it's for

**Legal aid clinics and self-help centers** — it's yours to run. Free, no license fee,
and without needing to talk to anyone first.

**Developers** — there's work worth doing. Start with the issues, or bring your own.

No signup, no waitlist. It's up.

---

*Built because the cost and complexity of being heard is where most people stop.*
