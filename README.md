<!--
author:   ICoBC - International Council on Badges and Credentials
email:    info@icobc.net
version:  1.0.0
language: en
narrator: UK English Female
comment:  A practical workshop course in which learners carry out a data protection impact assessment for a credential programme, minimise data, choose disclosure, expiry and status mechanisms, and document processor agreements and transfers, including AI processors.
@style
:root { --icobc-navy:#02375B; --icobc-orange:#F78222; --icobc-cyan:#5DCAE7; --icobc-lime:#B1CF37; --icobc-mist:#F1F5F8; --icobc-line:#D8E2E9; --icobc-muted:#4F6576; }
body { font-family: "Open Sans", Arial, sans-serif; }
h1, h2, h3, h4 { color: var(--icobc-navy); }
a { color: var(--icobc-navy); }
table th { background: var(--icobc-mist); color: var(--icobc-navy); }
blockquote { border-left: 4px solid var(--icobc-orange); background: var(--icobc-mist); padding: 8px 16px; }
@end
-->

# Privacy by Design for Credential Programmes

*A data protection impact assessment, done properly.*

## About this course

This course belongs to the ICoBC Credentialing Skills Framework (ICSF), skill SECP "Security, privacy and data protection" (VRITE pillar: Trustworthiness), at level L3 "Enable", stage A "Ability". At this level you perform privacy and security assessments for a programme and specify controls. At the Ability stage you practise that capability on realistic tasks, in a controlled setting such as a case.

**Who it is for**

- HR and learning technology owners (C3)
- Programme and micro-credential leads (E1)
- Education IT and credential operations (E4)
- Professional bodies and sector associations (P1)

**Prerequisite:** ICB-F10 Data Protection Basics for Credential Issuers. You should already know the basic data protection principles, the main roles (controller, processor) and the idea of a lawful basis.

**Learning outcomes.** After this course you can:

1. Carry out a data protection impact assessment for a credential programme.
2. Minimise data in public credentials and evidence.
3. Decide on selective disclosure, expiry and status mechanisms.
4. Document processor agreements and transfers.

**Workload.** This is a workshop with 6 hours of notional learning. This file covers the self-paced part. Live or workshop elements appear as facilitator notes.

**How it is assessed.** You complete a knowledge check of 10 questions and submit a data protection impact assessment (DPIA) for a real or case programme. A person assesses the DPIA with the rubric in the section "Assessment and badge". Nothing in this file grades your DPIA.

**Badge.** "Privacy by Design for Credential Programmes (Ability, L3)", alignment code ICSF-SECP-L3-A. The badge evidence is your DPIA document.

**Important limits.** This course supports good practice. It is not legal advice, and finishing it does not prove that you can do a particular job. Check the rules that apply in your jurisdiction and with your data protection officer.

| Outcome | Module | How it is assessed |
|---|---|---|
| 1. Carry out a data protection impact assessment for a credential programme | The DPIA step by step | Knowledge check; DPIA sections 1 to 4 and 7 |
| 2. Minimise data in public credentials and evidence | Minimisation | Knowledge check; DPIA section 5 |
| 3. Decide on selective disclosure, expiry and status mechanisms | Selective disclosure options; Privacy of status and revocation | Knowledge check; DPIA section 6 |
| 4. Document processor agreements and transfers | Contracts | Knowledge check; DPIA section 8 |

**Tracking the two contexts.** Worked examples run in two settings. In the first, a university's continuing education centre issues micro-credentials (cyan in the graphics, for education and providers). In the second, a corporate academy in an HR department issues internal and external skills badges (orange, for companies and employers). All numbers in examples are illustrative.

**Status of topics.** GDPR and data protection law are established and stable, but watch for changes proposed under the Digital Omnibus. Wallet protocols and credential formats (OpenID4VC, SD-JWT VC, ISO mdoc) are emerging: specified for the EUDI Wallet, while tooling and education profiles are still maturing. Status as of November 2026; check before publishing.

<!-- VERIFY: Confirm the current state of the Digital Omnibus proposals on data rules before publishing. -->

<details>
<summary>Facilitator notes</summary>

**Workshop shape (6 hours notional).** Suggested split: about 2.5 hours of self-paced reading and quizzes (this file), 2.5 hours of live practice in small groups, 1 hour for DPIA drafting and peer review.

- Before the session, ask participants to bring either a real programme (anonymised if needed) or choose one of the two case programmes in this file.
- Confirm that everyone completed ICB-F10 or has equivalent knowledge.
- Agree early how participants will submit the DPIA document and who assesses it.
- Remind the group that the course is vendor-neutral. Participants should describe functions, not products.

</details>

## The DPIA step by step

### Why a DPIA belongs in every credential programme

A credential programme collects, creates and shares personal data. Learners give names, contact details and identity checks. Assessors create results, comments and evidence files. The credential itself becomes a portable data record that the earner can show to many people for many years.

A data protection impact assessment (DPIA) is a structured process that describes a processing activity, judges its risks to the people affected, and decides what to do about those risks. In the GDPR, a DPIA is required where processing is likely to result in a high risk to individuals. Whether your programme crosses that line is a judgement you make and record, with your data protection officer where you have one.

<!-- VERIFY: Check the exact GDPR article numbers and wording on DPIA triggers before citing them in the final course; no article numbers are quoted here by design. -->

Credential programmes often raise the risk level for these reasons:

- Credentials are public or shareable, so a data record leaves your control.
- Evidence may include recordings, workplace products, assessor comments or special category data.
- Status checks may reveal when and where a credential is used.
- Automated tools, including AI, may score, summarise or flag learners.
- Employers, awarding bodies and platform operators all touch the data.

> A DPIA is a design tool. You start it when you design the programme, not after launch. The earlier you start, the cheaper the changes.

### The steps of a DPIA

This course uses eight steps. They follow the common pattern used by data protection authorities and the European Data Protection Board, simplified for credential work.

1. **Describe the programme and the processing.** What happens to data, from sign-up to expiry?
2. **Map the data and the people.** Which data items, which groups of people, which systems?
3. **Check necessity and proportionality.** Why do you need each item? Which lawful basis applies?
4. **Identify risks to people.** What could go wrong for the earner, not only for the organisation?
5. **Choose measures.** Minimisation, disclosure design, expiry, status privacy, security.
6. **Judge the residual risk.** What remains after the measures?
7. **Consult and record.** Involve the data protection officer, learners or their representatives where appropriate, and record advice and decisions.
8. **Review.** Set a date and triggers for review.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>The eight DPIA steps</title>
  <desc>A flow of eight labelled boxes in two rows. Row one: describe, map, necessity, risks. Row two: measures, residual risk, consult and record, review. An arrow from review returns to describe to show that the DPIA is revisited.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <g font-family="Open Sans, Arial, sans-serif" font-size="15" fill="#02375B" text-anchor="middle">
    <rect x="30" y="70" width="160" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
    <text x="110" y="105">1. Describe</text><text x="110" y="127">the processing</text>
    <rect x="220" y="70" width="160" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
    <text x="300" y="105">2. Map data</text><text x="300" y="127">and people</text>
    <rect x="410" y="70" width="160" height="80" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
    <text x="490" y="105">3. Necessity and</text><text x="490" y="127">proportionality</text>
    <rect x="600" y="70" width="170" height="80" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
    <text x="685" y="105">4. Identify risks</text><text x="685" y="127">to people</text>
    <rect x="600" y="270" width="170" height="80" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
    <text x="685" y="305">5. Choose</text><text x="685" y="327">measures</text>
    <rect x="410" y="270" width="160" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
    <text x="490" y="305">6. Judge</text><text x="490" y="327">residual risk</text>
    <rect x="220" y="270" width="160" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
    <text x="300" y="305">7. Consult</text><text x="300" y="327">and record</text>
    <rect x="30" y="270" width="160" height="80" rx="6" fill="#02375B" stroke="#02375B" stroke-width="2"/>
    <text x="110" y="305" fill="#FFFFFF">8. Review</text><text x="110" y="327" fill="#FFFFFF">and repeat</text>
  </g>
  <g stroke="#02375B" stroke-width="2" fill="none">
    <path d="M190 110 H220"/><path d="M380 110 H410"/><path d="M570 110 H600"/>
    <path d="M685 150 V270"/>
    <path d="M600 310 H570"/><path d="M410 310 H380"/><path d="M220 310 H190"/>
    <path d="M110 270 V210 H110 V150" stroke-dasharray="6 4"/>
  </g>
  <text x="400" y="420" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576" text-anchor="middle">Dashed line: step 8 returns to step 1 when the programme changes.</text>
</svg>

### Describing the processing: the credential life cycle

Step 1 is the step most teams rush. Describe the whole life cycle of the credential, not only the issuing moment. A useful frame has seven stages:

1. Enrolment and identity checks
2. Learning and assessment, including evidence
3. Decision to award
4. Issuing the credential to the earner
5. Sharing and verification by third parties
6. Status changes, expiry and revocation
7. Retention, archiving and deletion

For each stage, write down: who is involved, which data items appear, which systems and processors handle them, where the data is stored, and how long it stays. A one-page table is enough to start. Keep it factual. Do not write what you hope happens; write what happens.

**Worked example: University continuing education micro-credential**

The continuing education centre of a university plans a micro-credential in data literacy. Learners are adults, some of them employees whose employers pay the fees. The centre issues a digital credential through a hosted issuing service and keeps assessment evidence (a short project report and an assessor comment) in the learning platform.

The programme lead, Amara, starts the DPIA with the life cycle table:

| Stage | Data | Who | System | Retention (illustrative) |
|---|---|---|---|---|
| Enrolment | Name, email, date of birth, employer name | Admissions | Student record system | Length of study plus 6 years |
| Assessment | Project report, assessor comment, grade | Tutor, assessor | Learning platform | 2 years after award |
| Award | Decision, date | Exam board | Student record system | 6 years |
| Issue | Name, title, date, issuer, grade | Credential operations | Hosted issuing service | Until earner removes it |
| Verify | Credential data | Employers, recruiters | Public verification page | Until expiry |
| Status | Credential status | Issuer | Status service | Until expiry |
| Delete | All | Data owner | All | Per schedule |

Amara notices two gaps at once. The issuing service stores the date of birth, which the credential does not need. And nobody has set a retention period for the public verification page. Both go onto the DPIA risk list.

**Practice activity: Draft the life cycle table**

Choose a real credential programme you know, or use the corporate case below. In 15 minutes, draft a life cycle table with the seven stages. For each stage, fill in data, who, system and retention. Mark every cell you cannot fill with "unknown". Count the unknowns.

*Corporate case.* A corporate academy in an HR department issues a "Safe Data Handling" badge to all staff after an online course and a short scenario test. The badge is shown on the internal profile and learners may add it to a professional networking profile. Results are held in the company learning management system. A cloud-hosted issuing service creates the badge. An AI tool summarises free-text answers for the trainer.

Keep your table. You will extend it in the later modules and use it in your assessed DPIA.

### Necessity, proportionality and risk to people

Steps 3 and 4 turn the table into a judgement.

For **necessity and proportionality**, ask for each data item: what is the purpose, is the item needed for it, and is there a less intrusive way? Record the lawful basis for each purpose. In credential programmes the basis can differ by stage. Enrolment may rest on a contract with the learner. Publishing a credential on a public page may rest on the learner's consent or request. An employer's mandatory training record may rest on a legal obligation or on legitimate interests. Your ICB-F10 notes cover these bases; here you apply them stage by stage.

For **risks to people**, describe harm to the earner in plain words. Useful questions:

- Could someone identify or profile the earner from the credential or its status checks?
- Could a grade or a revocation cause discrimination, embarrassment or lost work?
- Could data be used for a purpose the earner did not expect?
- Could the earner lose control, for example by being unable to remove or correct data?

Rate each risk by likelihood and severity using a simple scale (low, medium, high) and say why. Keep the rating method the same across the DPIA so that readers can compare risks.

> Risks to the organisation, such as fines or reputation, matter, but a DPIA centres on risks to the people whose data you process.

<details>
<summary>Facilitator notes</summary>

- **Time:** 40 minutes live. 10 minutes to recap the eight steps, 20 minutes for the life cycle activity in pairs, 10 minutes to compare unknowns across pairs.
- Ask each pair to share their most surprising unknown. Common answers: retention of public pages, who the real processor is, where backups sit.
- Keep a flip chart of recurring risks. Use it again in Module 4.
- If participants bring real programmes, remind them not to share personal data of real learners.

</details>

### Check your understanding

**Question 1.** At which point in a credential programme should you start a DPIA?

[( )] After the first cohort has been issued, using real feedback
[(X)] During design, before the programme collects or issues data
[( )] Only when a complaint from an earner arrives
[( )] Only when the credential is shown to a third party
****
A DPIA is a design tool. Starting during design lets you change the programme cheaply. Starting later means retrofitting controls to data you already hold.
****

**Question 2.** Which description best fits step 4 of the DPIA, "identify risks"?

[( )] List the fines the organisation could face
[( )] Describe the technical architecture of the issuing service
[(X)] Describe what could go wrong for the earners and rate likelihood and severity
[( )] Select the vendor with the lowest price
****
The focus of the DPIA risk step is harm to individuals, rated with a consistent method. Fines, architecture and price are separate topics.
****

**Question 3.** Amara finds that the hosted issuing service stores the date of birth, although the credential does not show it. What is the best use of this finding in the DPIA?

[( )] Ignore it, because storage is cheap
[( )] Record it only as a security risk
[(X)] Record it as a necessity and proportionality issue and plan to remove the item
[( )] Move the date of birth to the public verification page
****
A data item that serves no purpose fails the necessity test. The best action is to record the finding and remove the item, which reduces risk at the source.
****

**Question 4.** Why should the life cycle table include the retention of the public verification page?

[( )] Because the verification page has no risks
[(X)] Because a public record can outlive its purpose and remain visible to anyone
[( )] Because retention periods apply only to public pages
[( )] Because the table must have exactly seven rows
****
Public pages are visible to many people and can live on indefinitely if nobody sets a limit. Retention is part of every stage, not only the first ones.
****

## Minimisation

### What minimisation means for credentials

Data minimisation means that you collect, hold and share only the personal data that you need for a stated purpose. In a credential programme, minimisation applies to three places:

- **The public credential.** What the credential shows to anyone who sees it or opens its link.
- **The evidence.** What you keep to prove that the earner met the criteria.
- **The records behind the scenes.** What the issuing platform and your own systems store.

Teams often put everything into the credential "to be safe": full name, date of birth, email, grade, employer, course code, assessor name, even a photo. Each extra item makes the credential more useful for tracking and more harmful if it leaks. A credential that carries a date of birth can also be used for identity fraud.

A simple test helps. For each item ask three questions:

1. Does a verifier need this to trust the credential?
2. Does the earner want to show this?
3. Would the earner be surprised to see it on a public page?

If the answers are no, no, yes, remove the item.

### Public credential, private evidence

Many programmes store evidence inside the credential, for example a link to a project report or a recording. A public link to evidence is a public disclosure of everything inside it. It may include other people's data, such as classmates in a group video or a client's name in a workplace project.

Good practice separates the two layers:

- The **credential** states the claim: who earned what, from whom, when, and the criteria in words.
- The **evidence** is held privately and shared only with people who have a reason, such as an assessor, an appeals panel, or a verifier the earner chooses.

Where evidence must be linked, protect the link with access control, and think about what happens when the link is shared further. Where it can be summarised, summarise it. A short statement such as "Project assessed against four criteria; all met" often says what the verifier needs.

Other minimisation moves:

- Use a person's name as they wish to show it, not necessarily the full legal name, unless identity assurance requires it.
- Avoid unique identifiers in public fields. An email address in a public credential invites scraping.
- Show a grade band only if grades are part of the claim.
- Avoid special category data (for example health or disability information) in any credential or public evidence. Reasonable adjustments in an exam do not belong on the badge.
- Think about metadata. Hidden fields, file properties and embedded images can leak more than the visible text.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>The same credential before and after minimisation</title>
  <desc>Two cards side by side. The left card, labelled before, lists nine data fields including date of birth, personal email, full grade breakdown, employer name and a link to a public project report. The right card, labelled after, lists four fields: display name, credential title, issuer and issue date, plus a status link with no personal data. A navy arrow points from left to right.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <g font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">
    <text x="40" y="40" font-size="16" font-weight="bold">Before: 9 fields</text>
    <rect x="30" y="55" width="330" height="340" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
    <text x="50" y="90">Full legal name</text>
    <text x="50" y="120">Date of birth</text>
    <text x="50" y="150">Personal email address</text>
    <text x="50" y="180">Employer name</text>
    <text x="50" y="210">Full grade breakdown</text>
    <text x="50" y="240">Assessor name and comment</text>
    <text x="50" y="270">Learner ID number</text>
    <text x="50" y="300">Public link to project report</text>
    <text x="50" y="330">Credential title and issuer</text>
    <text x="50" y="375" fill="#4F6576">Much of this is not needed to verify.</text>
    <path d="M375 225 H425" stroke="#02375B" stroke-width="2" fill="none"/>
    <path d="M415 215 L425 225 L415 235" stroke="#02375B" stroke-width="2" fill="none"/>
    <text x="440" y="40" font-size="16" font-weight="bold">After: 4 fields and a status link</text>
    <rect x="440" y="55" width="330" height="340" rx="6" fill="#FFFFFF" stroke="#02375B" stroke-width="2"/>
    <rect x="460" y="80" width="290" height="46" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
    <text x="475" y="109">Display name chosen by earner</text>
    <rect x="460" y="140" width="290" height="46" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
    <text x="475" y="169">Credential title and criteria</text>
    <rect x="460" y="200" width="290" height="46" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
    <text x="475" y="229">Issuer name</text>
    <rect x="460" y="260" width="290" height="46" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
    <text x="475" y="289">Issue date</text>
    <rect x="460" y="320" width="290" height="46" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
    <text x="475" y="349">Status link, no personal data</text>
  </g>
</svg>

### Minimising what the platform keeps

The credential is only the visible part. Behind it sit exports, logs, backups, analytics and support tickets. Include them in your minimisation review:

- **Issuing platform records.** Ask which fields the platform needs to issue and which it stores because the form had space. Remove optional fields you do not use.
- **Logs and analytics.** Verification logs can reveal where and when someone shows a credential. Set short retention and avoid storing IP addresses where you do not need them.
- **Backups and exports.** CSV files with learner lists spread quickly. Define who may export, where files go and when they are deleted.
- **Test data.** Use synthetic data for testing, not real learner records.

**Worked example: Minimising a corporate academy badge**

Jonas, learning technology owner at a corporate academy, reviews the "Safe Data Handling" badge. The first design shows full name, staff number, department, test score and the trainer's comment. The badge may be shared outside the company.

He applies the three questions and decides:

| Item | Decision | Reason |
|---|---|---|
| Full name | Keep, as the display name the employee prefers | Needed to link the claim to a person |
| Staff number | Remove | Identifies the employee inside the company; useless outside |
| Department | Remove | Reveals organisational information and is not part of the claim |
| Test score | Remove | Pass/fail is the claim; scores invite comparison |
| Trainer comment | Keep private | May contain personal remarks; keep in the learning record |
| Criteria text | Add | Helps the verifier understand what was assessed |

The final badge states: display name, "Safe Data Handling", the criteria in two sentences, issuer and issue date. Jonas records the decisions in the DPIA, with the reason for each removed item, so that the reasoning survives staff changes.

**Practice activity: Minimise a credential**

Take the micro-credential from the university case (Module 1) with this current design: full legal name, date of birth, personal email, employer name, grade (as a percentage), assessor name, a public link to the project report, and the credential title.

1. Apply the three questions to every item and make a table like Jonas's.
2. Decide what the public credential shows, what stays in private evidence, and what the platform should not store.
3. Write two sentences for the DPIA that justify your decisions.

Compare your result with a partner. Where you disagree, ask what the earner would expect.

<details>
<summary>Facilitator notes</summary>

- **Time:** 45 minutes live. 5 minutes introduction, 20 minutes for the activity in small groups, 20 minutes for the debrief.
- Good debrief question: "Which item did the most groups disagree about?" Typical answers: the grade, the employer name, the assessor name.
- Highlight that "the employer paid" is not a reason to put the employer name on a credential the earner owns.
- Show a before and after card on the screen using the graphic in this module.
- Reminder: pass/fail claims and grade bands can both be valid. The point is to justify the choice.

</details>

### Check your understanding

**Question 1.** Which question is part of the three-question minimisation test?

[( )] Does the platform have a field for it?
[( )] Do other issuers include it?
[(X)] Does a verifier need this to trust the credential?
[( )] Was it in the previous version of the credential?
****
The test asks whether a verifier needs the item, whether the earner wants to show it, and whether the earner would be surprised to see it. Habit and platform fields are not reasons.
****

**Question 2.** A credential links to a public project report that names two clients. What is the main privacy concern?

[( )] The report is too long to read
[(X)] The link discloses the report and the clients' data to anyone who finds it
[( )] The earner cannot download the report
[( )] The report format is outdated
****
A public link discloses everything inside the report, including other people's data. Keeping evidence private, or summarising it, removes the problem.
****

**Question 3.** Which data should normally never appear in a public credential?

[( )] The credential title
[( )] The issuer name
[( )] The issue date
[(X)] Information about a learner's disability adjustments
****
Special category data such as health or disability information does not belong in a public credential. The other items are core parts of the claim.
****

**Question 4.** Jonas removes the staff number from the badge. Which reason fits best?

[( )] Staff numbers are always secret
[(X)] The number identifies the employee inside the company and adds no value outside it
[( )] Badges may only have four fields
[( )] Staff numbers confuse the issuing platform
****
The number links the badge to an internal record and helps tracking, but it does not help an outside verifier. That fails the necessity test.
****

**Question 5.** Which place is easy to forget in a minimisation review?

[( )] The credential title
[(X)] Verification logs, exports and backups behind the platform
[( )] The programme name
[( )] The issuer logo
****
Logs, exports and backups hold personal data and are often kept longer than anyone intends. They belong in the review.
****

## Selective disclosure options

### What selective disclosure is

Selective disclosure lets an earner reveal only part of a credential to a verifier. A student who needs to prove "has completed a data literacy micro-credential" does not need to show the grade, the date of birth or the assessor's name. The earner chooses which claims to show, and the verifier can still check that the issuer signed them.

Selective disclosure complements minimisation. Minimisation decides what goes into the credential. Selective disclosure decides what leaves the wallet in each presentation.

Three questions drive the design:

1. **What does the verifier need to know?** Often a fact, such as "holds the badge" or "passed", rather than the full record.
2. **Who holds the credential?** A wallet controlled by the earner, a platform account, or a PDF in an inbox.
3. **How should the verifier check it?** By the issuer's signature, by a status check, or by calling the issuer.

### Options at a glance

A credential programme can choose from several options. They differ in privacy, effort and tool support.

| Option | What the verifier sees | Privacy strength | Notes |
|---|---|---|---|
| Public page with all claims | Everything, to anyone with the link | Low | Easy, but hard to withdraw |
| Public page with minimal claims | Only the minimal claim | Medium | Combine with minimisation |
| Private link or access code | Everything, to link holders | Medium | The earner shares and can revoke the link |
| Signed credential in a wallet, full presentation | All claims, to the chosen verifier | Medium to high | The earner chooses the verifier |
| Signed credential with selective disclosure | Only claims the earner selects | High | Needs format and wallet support |
| Derived attribute (for example "over the threshold") | A yes/no result | High | Needs issuer and verifier agreement |

Formats such as SD-JWT VC and ISO mdoc support selective disclosure of individual claims. OpenID4VC protocols describe how a wallet and a verifier exchange credentials. These specifications are used for the EUDI Wallet. Tooling and education-specific profiles are still maturing, so this part of the field is emerging. Check the current state of the specifications and your tools before committing to a design.

<!-- VERIFY: Check the current status of SD-JWT VC, ISO mdoc and OpenID4VC specifications and of any education profiles before publishing. -->

You do not need to master the cryptography to make a good decision. You need to know what each option lets the verifier see, and what it lets the verifier learn over time.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Selective disclosure between issuer, earner and verifier</title>
  <desc>Three boxes in a row. An issuer box on the left (cyan) signs a credential with four claims and sends it to an earner wallet in the centre (navy). The earner selects two claims and sends them to a verifier box on the right (orange). The verifier checks the issuer signature. Two claims stay hidden in the wallet.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <g font-family="Open Sans, Arial, sans-serif" font-size="15" fill="#02375B" text-anchor="middle">
    <rect x="30" y="140" width="190" height="150" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
    <text x="125" y="175" font-weight="bold">Issuer</text>
    <text x="125" y="205">Signs a credential</text>
    <text x="125" y="228">with four claims</text>
    <rect x="305" y="110" width="190" height="210" rx="6" fill="#02375B" stroke="#02375B" stroke-width="2"/>
    <text x="400" y="145" fill="#FFFFFF" font-weight="bold">Earner wallet</text>
    <rect x="325" y="165" width="150" height="34" rx="6" fill="#FFFFFF" stroke="#B1CF37" stroke-width="2"/>
    <text x="400" y="188">Claim A: shown</text>
    <rect x="325" y="207" width="150" height="34" rx="6" fill="#FFFFFF" stroke="#B1CF37" stroke-width="2"/>
    <text x="400" y="230">Claim B: shown</text>
    <rect x="325" y="249" width="150" height="26" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
    <text x="400" y="267" font-size="14" fill="#4F6576">Claim C: hidden</text>
    <rect x="325" y="281" width="150" height="26" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
    <text x="400" y="299" font-size="14" fill="#4F6576">Claim D: hidden</text>
    <rect x="580" y="140" width="190" height="150" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
    <text x="675" y="175" font-weight="bold">Verifier</text>
    <text x="675" y="205">Receives claims A, B</text>
    <text x="675" y="228">Checks issuer signature</text>
  </g>
  <g stroke="#02375B" stroke-width="2" fill="none">
    <path d="M220 215 H305"/><path d="M295 205 L305 215 L295 225"/>
    <path d="M495 215 H580"/><path d="M570 205 L580 215 L570 225"/>
  </g>
  <g font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576" text-anchor="middle">
    <text x="262" y="200">Issue</text>
    <text x="537" y="200">Present</text>
    <text x="400" y="400">The earner chooses what to present. The verifier cannot see hidden claims.</text>
  </g>
</svg>

### Expiry as a privacy tool

Every credential has a life. Expiry is a way to end the exposure of data and to keep claims honest. Decide for each credential type:

- **Does the claim go stale?** A safety training badge may need renewal. A degree does not expire in the same way.
- **What does expiry do to the data?** Expiry should reduce visibility, for example by ending the public page or ending the validity period inside the credential, not merely adding a date in a footnote.
- **What happens to data after expiry?** Decide whether the issuer keeps a record of the award, and for how long, for a stated purpose such as handling disputes.

Separate three ideas that teams often mix:

- **Validity period:** the period in which the claim is current.
- **Expiry of the public presentation:** when the link or page stops working.
- **Retention of the issuer's record:** how long you keep your own data about the award.

A micro-credential might have no validity end, a public page that the earner can remove at any time, and an issuer record kept for six years (illustrative). Write each decision down and give a reason.

> Choose the simplest mechanism that meets the verifier's need. A fancy format does not repair a credential that contains data nobody needed to show.

**Worked example: Choosing a disclosure design at the university**

The continuing education centre of the university serves two main verifiers: employers, who want to confirm that the micro-credential exists and is current, and other universities, who sometimes want the grade for credit transfer.

Amara lists the needs:

| Verifier | Needs | Does not need |
|---|---|---|
| Employer | Title, issuer, date, valid | Grade, assessor, date of birth |
| Receiving university | Title, issuer, date, grade band | Employer name, personal email |

She proposes a design for the DPIA. The earner holds a signed credential that contains title, issuer, date, grade band and a status reference. Where the tools support selective disclosure, the earner shows title, issuer and date to employers and adds the grade band for universities. Where the tools do not yet support it, the centre issues a public page with minimal claims (title, issuer, date) and a separate private link for the grade band that the earner can switch off.

She records the reason: the second option is a fallback because tooling for education profiles is still maturing, and she sets a review date to revisit the design.

**Practice activity: Pick a disclosure design**

Use the corporate case (Safe Data Handling badge). The audiences are: (a) the employee's manager, (b) an external client who asks for proof of training before a contract, (c) a recruiter reading the employee's professional networking profile.

1. For each audience, list what they need and what they do not need.
2. Choose one option from the table in this module for each audience and justify it in one sentence.
3. Decide on validity period, public page expiry and issuer record retention. Use illustrative numbers and say they are illustrative.
4. Note which of your choices depend on tools that may not yet exist in your organisation.

<details>
<summary>Facilitator notes</summary>

- **Time:** 50 minutes live. 10 minutes on the options table, 25 minutes for the activity in groups of three, 15 minutes for the debrief.
- If a technical colleague is present, invite a short demonstration of how selective disclosure appears in a wallet interface, using any open specification demo. Keep it vendor-neutral.
- Stress that the correct answer depends on the verifier's real need. A group that picks "wallet with selective disclosure" for everything has probably skipped the need analysis.
- Ask: "What happens to your design if the wallet tool is not available in two years?"

</details>

### Check your understanding

**Question 1.** What is the main purpose of selective disclosure?

[( )] To make the credential look more attractive
[(X)] To let the earner show only the claims a verifier needs
[( )] To remove the issuer's signature
[( )] To store the credential on the issuer's server only
****
Selective disclosure lets the earner choose which claims leave the wallet, while the verifier can still check the issuer's signature on what is shown.
****

**Question 2.** An employer needs to confirm that a micro-credential exists and is current. Which design fits the need best?

[( )] A public page with the full grade breakdown and evidence
[( )] A PDF containing the date of birth to prove identity
[(X)] A presentation of title, issuer, date and a status check, without the grade
[( )] A phone call to the earner's friends
****
The employer needs existence and currency. Title, issuer, date and status answer that. The grade and evidence are not needed.
****

**Question 3.** Which statement about OpenID4VC, SD-JWT VC and ISO mdoc is the most accurate for this course?

[( )] They are mature, with complete education profiles in all tools
[( )] They are banned for credential programmes
[(X)] They are specified for the EUDI Wallet, while tooling and education profiles are still maturing
[( )] They replace the need for a DPIA
****
These specifications are emerging for credentials. Plan for a fallback and set review dates. No technology replaces a DPIA.
****

**Question 4.** Which pair correctly separates two ideas about the life of a credential?

[( )] Validity period and the colour of the badge
[(X)] Validity period of the claim and retention of the issuer's own record
[( )] Issue date and the file name
[( )] Public page expiry and the issuer logo
****
The claim's validity period, the end of public presentation and the issuer's retention of its record are separate decisions, each with its own reason.
****

## Privacy of status and revocation

### Why status needs its own look

A credential can change state. It can be valid, suspended, revoked, expired or replaced. Verifiers want to know the current state, so many systems offer a status check. That check is a data flow in its own right, and it can reveal information about the earner.

Think about what a simple status check does. A verifier opens a link or calls a service, and the issuer's server sees that the check happened. The server may learn the time, the verifier's network address, and which credential was checked. Over time that creates a record of where and when the earner shows the credential. If the status entry is public, other people may also learn that a credential was revoked, which can say something about the earner.

Two privacy risks stand out:

- **Phone-home tracking.** The issuer learns when and where a credential is used.
- **Status leakage.** The status itself reveals sensitive facts, for example that a professional licence was suspended.

### Design choices for status

You can reduce these risks through design. Common approaches include:

| Approach | How it works | Privacy effect |
|---|---|---|
| Per-credential status page | A unique URL per credential returns the state | Simple, but the issuer sees each check and the page may be public |
| Status list | Many credentials share one list; each has a position in it | The issuer cannot easily tell which credential was checked, and the list does not name earners |
| Short-lived credentials | The credential expires soon and is reissued | Fewer status checks needed, but more issuing events |
| Offline verification | The verifier checks the signature only | No phone-home, but cannot see revocation |
| Issuer-hosted dashboard for the earner | The earner sees and controls their own status and who checked | Gives the earner transparency |

Status lists in the style described by public specifications, including the work on credential status in OpenID4VC and W3C-related communities, aim to hide which credential a verifier checks. Check the current specifications and your tools before relying on a particular mechanism.

<!-- VERIFY: Confirm the current names and status of credential status list specifications before citing them in the final course. -->

Choose the mechanism by balancing three needs: the verifier's need for current information, the earner's need for privacy, and the issuer's need for control. For low-stakes participation badges, offline verification may be enough. For credentials that give a right to practise or access, the verifier needs reliable revocation.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Two status check designs compared</title>
  <desc>Two panels. The left panel shows a verifier asking the issuer about one specific credential, so the issuer sees which credential was checked. The right panel shows a verifier downloading a shared status list with many entries, so the issuer cannot tell which entry was read. Both panels are labelled and use text as well as colour.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <g font-family="Open Sans, Arial, sans-serif" font-size="15" fill="#02375B" text-anchor="middle">
    <text x="200" y="40" font-weight="bold">Per-credential status check</text>
    <rect x="30" y="70" width="140" height="80" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
    <text x="100" y="105">Verifier</text><text x="100" y="127">asks about #4821</text>
    <rect x="240" y="70" width="140" height="80" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
    <text x="310" y="105">Issuer sees</text><text x="310" y="127">which credential</text>
    <path d="M170 110 H240" stroke="#02375B" stroke-width="2" fill="none"/>
    <path d="M230 100 L240 110 L230 120" stroke="#02375B" stroke-width="2" fill="none"/>
    <text x="200" y="200" fill="#4F6576">Risk: the issuer can log</text>
    <text x="200" y="222" fill="#4F6576">when and where it is used.</text>
    <text x="600" y="40" font-weight="bold">Status list check</text>
    <rect x="430" y="70" width="140" height="80" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
    <text x="500" y="105">Verifier</text><text x="500" y="127">fetches whole list</text>
    <rect x="640" y="70" width="140" height="80" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
    <text x="710" y="105">Issuer serves</text><text x="710" y="127">a shared list</text>
    <path d="M570 110 H640" stroke="#02375B" stroke-width="2" fill="none"/>
    <path d="M630 100 L640 110 L630 120" stroke="#02375B" stroke-width="2" fill="none"/>
    <rect x="450" y="250" width="300" height="60" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
    <text x="600" y="278">List of many entries</text>
    <text x="600" y="298" font-size="14" fill="#4F6576">No names, one position per credential</text>
    <text x="600" y="200" fill="#4F6576">Better: the issuer cannot tell</text>
    <text x="600" y="222" fill="#4F6576">which entry was read.</text>
    <path d="M200 270 V330" stroke="#D8E2E9" stroke-width="2" fill="none"/>
    <text x="400" y="400" fill="#4F6576">Both designs still need retention limits for logs.</text>
  </g>
</svg>

### Revocation rules and fairness

Privacy of status is also about fairness. A revocation is a serious event. Write clear rules before launch:

- **Reasons.** List the reasons for suspension and revocation, such as error in issuing, finding of misconduct, or fraud. Avoid vague wording.
- **Process.** Say who decides, how the earner is told, and how they can challenge the decision.
- **Visibility.** Decide what a verifier sees: "not valid" without a reason is usually enough. Do not publish the reason.
- **Records.** Keep the evidence of the decision privately, with a retention period.
- **Reissue.** Explain how a credential can be restored or replaced.

If automated tools assist in decisions, for example a tool that flags suspected plagiarism, ensure that a person reviews any outcome that affects the earner. Record this in the DPIA.

Another point is the **right to be forgotten** and the **right to erasure**. A credential an earner holds is under the earner's control. Your DPIA should say what happens when the earner asks you to delete data: you can remove your own records and public pages where no overriding reason exists, but you cannot erase a copy that the earner or a verifier holds. Make this limit clear to earners in the privacy information.

**Worked example: Status design at the corporate academy**

Jonas's "Safe Data Handling" badge is valid for two years, after which staff must renew it. The badge is also used when staff visit client sites. The original design gives each badge a unique status URL on the issuing service. Jonas notices that the service logs the network address of each verifier and the badge number. That would let the vendor and the academy see which client checked which employee's badge and when.

He changes the design:

- Use a shared status list so that individual checks are not tied to a person in the logs.
- Cut verification log retention to a short period (illustrative: 30 days) and keep no network addresses.
- Make the validity period two years inside the badge, so offline checks give a reasonable answer.
- Publish only "valid" or "not valid" to verifiers.
- Write revocation rules: revocation for issuing errors or a confirmed breach of the training policy, with notice to the employee and a route to appeal through HR.

He records in the DPIA that a person in HR reviews any revocation, and that the AI summarising tool plays no role in revocation decisions.

**Practice activity: Review a status design**

Take the university micro-credential. The current design uses a unique public status page for each credential and logs the network address and time of every check. The page also shows "Revoked: plagiarism finding" when a credential is revoked.

1. List at least three privacy problems.
2. Redesign the status mechanism. Choose one approach from the table and say why.
3. Write three short revocation rules (reason, process, visibility).
4. Add two lines to the DPIA risk register: one on status tracking, one on status leakage.

<details>
<summary>Facilitator notes</summary>

- **Time:** 45 minutes live. 10 minutes on the table of approaches, 20 minutes for the activity, 15 minutes for the debrief.
- Common problems participants find: the reason for revocation is public, logs keep network addresses, no appeal route, status page is indexed by search engines.
- Ask participants to role-play the earner who finds their revoked credential online. What would they feel? What would they ask?
- Reinforce that revocation rules protect the earner and the issuer alike.
- Link this module back to the DPIA risk step: status tracking and status leakage are typical entries.

</details>

### Check your understanding

**Question 1.** What is the main privacy risk of a unique status page for each credential?

[( )] The page loads slowly
[(X)] The issuer can learn when and where each credential is checked
[( )] The credential title is too long
[( )] The page is always correct
****
A per-credential check shows the issuer which credential was checked, and logs can build a picture of where and when the earner uses it.
****

**Question 2.** What is the advantage of a shared status list?

[( )] It names every earner in public
[( )] It removes the need to revoke credentials
[(X)] The issuer cannot easily tell which entry a verifier read, and the list holds no names
[( )] It replaces the credential
****
A shared list hides which credential was checked and carries positions rather than names. Logs still need retention limits.
****

**Question 3.** What should a verifier normally see when a credential is revoked?

[( )] The full reason, including any misconduct finding
[(X)] That the credential is not valid, without the reason
[( )] The earner's home address
[( )] The assessor's private notes
****
Publishing the reason can harm the earner and goes beyond what a verifier needs. Keep reasons in the private record.
****

**Question 4.** An AI tool flags a learner for suspected plagiarism. What should the DPIA say about revocation?

[( )] The AI decision is final
[( )] The learner is told only after the credential is revoked
[( )] The tool's output is published on the status page
[(X)] A person reviews the flag before any outcome affects the learner, and the learner can challenge the decision
****
Outcomes that affect the earner need human review and a route to challenge. The DPIA should record this and treat the AI tool as a processor or system within scope.
****

## Contracts

### Controllers, processors and joint controllers

A credential programme rarely runs on one organisation's systems alone. A university may use a hosted learning platform, an issuing service, an identity verification provider, and an AI tool that summarises evidence. A corporate academy may add a cloud learning management system and a professional networking site. Each organisation that touches personal data has a role.

Recall the basic roles from ICB-F10:

- The **controller** decides why and how personal data is processed.
- The **processor** processes personal data on behalf of the controller and follows its instructions.
- **Joint controllers** decide together on purposes and means.
- A **sub-processor** is a processor that your processor hires.

Roles come from what organisations actually do, not from what the contract calls them. A provider that decides on its own to use learner data to train its own models is acting as a controller for that use, whatever the contract says. Your DPIA must name the role of each party and check that the paperwork matches reality.

When you use a processor, data protection law requires a written contract or other legal act that sets out the subject matter, duration, nature and purpose of processing, the type of personal data, the categories of people, and the controller's rights and duties. It also contains obligations for the processor, such as processing only on documented instructions, confidentiality, security, support for people's rights, help with the DPIA, rules on sub-processors, and deletion or return of data at the end.

<!-- VERIFY: Check the exact GDPR article numbers and the list of mandatory processor contract terms before citing them in the final course; none are quoted here by design. -->

### What to check in a processor agreement

Use a checklist. For each processor, confirm:

1. **Scope.** Which data, which people, which purposes, how long.
2. **Instructions.** The processor acts only on your documented instructions. No own-purpose use, including model training, unless you agreed and have a basis.
3. **Security.** Technical and organisational measures are described and match your risk.
4. **Sub-processors.** A list, a notice process for changes, and a right to object.
5. **Location and access.** Where data is stored and who can access it, including support staff in other countries.
6. **Rights and incidents.** Support for access, correction and deletion requests, and a time limit for notifying you of a personal data breach.
7. **Audit.** The right to evidence and audits proportionate to risk.
8. **End of service.** Return or deletion of data, including backups, with confirmation.

Check also the **technical reality**. Does the platform let you delete a single learner's data? Can you set retention? Can you switch off analytics? A contract that promises deletion is of little use if the platform cannot do it.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Data flows and roles in a credential programme</title>
  <desc>A diagram with a central navy circle labelled earner. Around it are an education provider as controller in cyan, an employer as separate controller in orange, a hosted issuing service as processor, an AI summarising tool as processor or sub-processor, and a standards and policy body in lime outside the data flow. Arrows show personal data moving from the provider to the processors and to the earner. A dashed border marks a transfer outside the European Economic Area.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <g font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B" text-anchor="middle">
    <circle cx="400" cy="225" r="60" fill="#02375B"/>
    <text x="400" y="222" fill="#FFFFFF" font-weight="bold">Earner</text>
    <text x="400" y="242" fill="#FFFFFF">data subject</text>
    <rect x="40" y="60" width="200" height="80" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
    <text x="140" y="95" font-weight="bold">Education provider</text>
    <text x="140" y="117">Controller</text>
    <rect x="560" y="60" width="200" height="80" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
    <text x="660" y="95" font-weight="bold">Employer or verifier</text>
    <text x="660" y="117">Own controller</text>
    <rect x="40" y="310" width="200" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
    <text x="140" y="345" font-weight="bold">Hosted issuing service</text>
    <text x="140" y="367">Processor</text>
    <rect x="300" y="340" width="200" height="80" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2" stroke-dasharray="8 4"/>
    <text x="400" y="375" font-weight="bold">AI summarising tool</text>
    <text x="400" y="397">Processor, outside EEA</text>
    <rect x="560" y="310" width="200" height="80" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
    <text x="660" y="345" font-weight="bold">Policy and standards</text>
    <text x="660" y="367">Rules, not data flow</text>
  </g>
  <g stroke="#02375B" stroke-width="2" fill="none">
    <path d="M240 100 L345 195"/>
    <path d="M560 100 L455 195"/>
    <path d="M140 140 V310"/>
    <path d="M200 140 L330 340" stroke-dasharray="6 4"/>
  </g>
  <text x="400" y="30" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576" text-anchor="middle">Dashed lines: transfer outside the European Economic Area, which needs a transfer mechanism.</text>
</svg>

### Transfers and AI processors

A **transfer** happens when personal data goes to a country outside the area where the main data protection regime applies, or becomes accessible from there. Under the GDPR, transfers outside the European Economic Area need a recognised mechanism, such as an adequacy decision or appropriate safeguards, and you must assess the circumstances of the transfer. Remote access by a support team in another country can count as a transfer.

<!-- VERIFY: Check the current list of adequacy decisions and the status of any transfer frameworks before publishing; none are named here by design. -->

Document each transfer in your DPIA: the data, the sender, the recipient, the country, the mechanism, and any extra measures such as encryption where the provider does not hold the keys. If you cannot name the mechanism, the transfer is a risk. Consider whether you can avoid the transfer by choosing another provider or region.

**AI processors need their own line in the DPIA.** An AI tool that summarises evidence, scores free-text answers, flags suspected plagiarism or matches skills to roles processes personal data and may influence decisions about people. Ask:

- **Role and purpose.** Is the AI provider a processor? Is it allowed to use your data for its own purposes, such as improving models? The default answer in your contract should be no.
- **Data in prompts and outputs.** Which personal data goes in? Do outputs contain personal data? Where are inputs, outputs and logs stored, and for how long?
- **Accuracy and bias.** How do you check that outputs are fair and correct? Which groups might be disadvantaged?
- **Human oversight.** Does a person make the decision? Can the earner challenge it? Rules on automated decision-making may apply where a decision has legal or similarly significant effects.
- **Transparency.** Do earners know that AI is used and why?
- **Sub-processors and location.** The AI provider may use further infrastructure providers in other countries. List them.
- **Minimisation.** Can you remove names and identifiers before sending text to the tool?

Rules on AI systems are developing. Check what applies to your programme and your jurisdiction with your legal adviser.

<!-- VERIFY: Check which EU AI rules apply to education and employment uses of AI at the time of publishing; no specific provisions or dates are stated here by design. -->

**Worked example: Contracts and transfers at the university**

Amara lists the parties in the micro-credential programme:

| Party | Role | Data | Location (illustrative) | Contract status |
|---|---|---|---|---|
| University | Controller | All | Home country | n/a |
| Hosted issuing service | Processor | Name, title, date, grade band | Within the EEA | Agreement signed, sub-processor list missing |
| Learning platform | Processor | Evidence, comments | Within the EEA | Agreement signed, deletion process unclear |
| AI summarising tool | Processor | Project reports (text) | Outside the EEA | No agreement yet |
| Employers | Own controllers when they receive credential data | Credential data shown by the earner | Various | Not applicable; privacy notice to earners |

She records four actions in the DPIA: request the sub-processor list from the issuing service; ask the learning platform to demonstrate single-learner deletion; pause use of the AI tool until an agreement states that learner data is not used to train the provider's models, the transfer mechanism is documented, and names are removed before text is sent; and tell earners in the privacy notice which parties receive their data and that employers who receive a credential act as their own controllers.

**Practice activity: Build a processor and transfer register**

Use the corporate case. The academy uses a cloud learning management system, a hosted issuing service, an AI tool that summarises free-text answers and a professional networking site where staff may share the badge.

1. Make a register with columns: party, role, data, location, contract or mechanism, open actions. Use "unknown" where the case does not say.
2. For the AI tool, answer the seven questions in this module in one line each.
3. Decide which party is a processor and which is a separate controller. Explain the networking site in one sentence.
4. List the three most urgent actions and who owns each.

<details>
<summary>Facilitator notes</summary>

- **Time:** 55 minutes live. 10 minutes on roles, 25 minutes for the register activity, 20 minutes for the debrief and a first look at the assessed DPIA.
- Invite a procurement or legal colleague to answer questions, if possible. Remind everyone that the course gives no legal advice.
- Typical mistakes: calling the networking site a processor, forgetting support access from other countries, forgetting AI provider logs.
- Ask: "Which clause in the contract would you change first, and what would you do if the provider refuses?"
- Use the last 10 minutes to remind participants of the assessed DPIA and the rubric. Ask them to pick their programme now.

</details>

### Check your understanding

**Question 1.** A provider decides by itself to use learner data to train its own models. What is its role for that use?

[( )] Processor, because the contract says so
[(X)] Controller for that use, because it decides purposes and means
[( )] Data subject
[( )] Sub-processor of the learner
****
Roles follow what organisations actually do. A party that decides its own purposes acts as a controller for them, whatever label the contract carries.
****

**Question 2.** Which item belongs on a processor agreement checklist?

[( )] The colour of the provider's logo
[(X)] Sub-processors, with a notice process and a right to object
[( )] The number of staff the provider employs
[( )] The provider's marketing plan
****
Sub-processors extend the chain of processing. The controller needs to know who they are and to be told about changes.
****

**Question 3.** Remote access by a support team in another country to learner data stored in the EEA is best treated as what?

[( )] Not relevant, because the data is stored in the EEA
[( )] An automatic breach
[(X)] A possible transfer that you document and assess with the provider
[( )] A reason to publish the data
****
Access from another country can count as a transfer. Document it and check the mechanism and any extra measures.
****

**Question 4.** Which question belongs in the DPIA entry for an AI summarising tool?

[( )] Does the tool have a friendly name?
[(X)] Is the provider allowed to use inputs and outputs for its own purposes, and where are they stored?
[( )] How many languages does the tool speak?
[( )] Which colour is its interface?
****
Use of data for the provider's own purposes, and the storage of inputs, outputs and logs, are core privacy questions for any AI processor.
****

## Assessment and badge

### The assessed task: a DPIA for a programme

You carry out a data protection impact assessment for a real or case programme and submit it as a document. The document is the badge evidence. A person assesses it with the rubric below. Nothing in this file grades the DPIA.

**Choose your programme.** Use a real credential programme you work with (anonymise personal data and confidential details), or use one of the two cases in this course (the university micro-credential or the corporate Safe Data Handling badge) and extend it with realistic detail.

**Required structure.** Your DPIA contains these eight sections. Aim for 6 to 12 pages in total.

1. **Programme description and purposes.** Aims, audience, credential types, life cycle table (Module 1).
2. **Data and people map.** Data items, groups of people, systems, locations.
3. **Necessity, proportionality and lawful basis.** For each purpose and stage.
4. **Risks to people.** A risk register with likelihood, severity and rating method.
5. **Minimisation decisions.** Public credential, evidence and platform records, with reasons (Module 2).
6. **Disclosure, expiry and status.** Your chosen design, the reasons, retention of logs and revocation rules (Modules 3 and 4).
7. **Measures, residual risk and consultation.** Measures per risk, residual rating, advice from the data protection officer or a named equivalent, and a review date.
8. **Processors, AI and transfers.** A register of parties, roles, contract status and transfer mechanisms, with a specific entry for any AI processor (Module 5).

Label any assumption as an assumption. Where you cannot decide, say who must decide and by when.

### Rubric

Each criterion is rated 1 (not yet), 2 (meets), or 3 (strong). The assessor adds a short written comment for each criterion.

| Criterion | 1: Not yet | 2: Meets | 3: Strong |
|---|---|---|---|
| A. Describing the processing (outcome 1) | Life cycle is partial or vague; many items unknown | Whole life cycle covered; data, people, systems and retention stated | Complete, accurate and checked against real or realistic practice; unknowns are listed with owners |
| B. Necessity, lawful basis and risk (outcome 1) | Purposes or bases missing; risks focus on the organisation only | Purposes and bases stated per stage; risks to people rated with a stated method | Bases differ by stage with reasons; risks are specific, rated consistently and linked to measures |
| C. Minimisation (outcome 2) | Items kept without reasons; evidence stored publicly | Each item justified; evidence kept private or summarised; platform records reviewed | Clear before and after view; logs, exports and metadata covered; reasons would survive a challenge |
| D. Disclosure, expiry and status (outcome 3) | Design chosen without reference to verifier needs; status privacy ignored | Design matched to verifier needs; expiry, status and revocation rules stated | Options compared; fallbacks for immature tooling stated; revocation fairness and log retention addressed |
| E. Processors, AI and transfers (outcome 4) | Parties or roles missing; transfers undocumented | Register complete; roles and contract status stated; transfers have a mechanism or an action | Role assessment tested against actual practice; AI processor covered in depth; open actions have owners and dates |
| F. Residual risk, consultation and review (outcome 1) | No residual rating, advice or review date | Residual risk stated; advice recorded; review date and triggers set | Residual risk justified; unresolved risks escalated; review triggers are specific |
| G. Clarity and use of sources | Hard to follow; claims unsupported | Clear structure; claims tied to named public sources or marked as assumptions | Concise and well organised; limits and legal checks flagged honestly |

**Pass rule.** To earn the badge you need all of the following:

- a rating of at least 2 on every criterion A to G,
- at least four ratings of 3 are not required, but any rating of 1 means the DPIA is returned with comments for revision, and
- a score of at least 8 out of 10 on the knowledge check below (the questions are in this file, and the knowledge check is self-marked using the explanations).

One resubmission is allowed after revision. The assessor may ask short clarifying questions about your DPIA.

**Evidence submitted for the badge.** Your DPIA document, with section 1 to 8, and the assessor's written rubric comments. The badge is "Privacy by Design for Credential Programmes (Ability, L3)", alignment code ICSF-SECP-L3-A. Holding it shows that you completed this course and had a DPIA assessed. It does not by itself prove competence in a particular job.

<details>
<summary>Facilitator notes</summary>

- **Time:** allow about 60 minutes in the workshop for drafting and peer review. The full DPIA may be finished after the session within an agreed period.
- Agree one assessor per DPIA. If possible, use a second assessor to sample at least one DPIA in five for consistency.
- Calibrate with a short sample: show an extract (for example one risk register row) and ask assessors to rate it against the rubric.
- Give written feedback for each criterion. For a rating of 1, say what the learner should change.
- Do not collect real personal data of learners in the submitted documents. Ask for anonymisation.
- Record the assessment result and the date. Issue the badge when the pass rule is met.

</details>

### Final knowledge check

Answer all 10 questions. Check the explanation after each one.

**Question 1.** A team starts a DPIA two weeks after launching the programme, because a complaint arrived. What is the best description of this?

[( )] Good practice, because real data is available
[(X)] Late: a DPIA should start during design, when changes are cheapest
[( )] Compliant, because a DPIA is only needed after complaints
[( )] Unnecessary, because credentials contain little data
****
A DPIA is a design tool. Starting during design lets you change the programme before data flows. Starting after launch means retrofitting.
****

**Question 2.** Which sequence matches the eight DPIA steps in this course?

[( )] Review, measures, describe, risks, necessity, map, record, residual risk
[(X)] Describe, map, necessity, risks, measures, residual risk, consult and record, review
[( )] Measures, describe, review, risks, map, record, necessity, residual risk
[( )] Describe, review, map, measures, risks, necessity, record, residual risk
****
The course sequence runs from describing the processing, through mapping, necessity, risks, measures and residual risk, to consultation, recording and review.
****

**Question 3.** In a DPIA risk register, which entry is written from the right perspective?

[( )] "The organisation may lose reputation if a complaint is published."
[( )] "The platform may be expensive."
[(X)] "An earner could be identified and profiled from repeated status checks of their credential."
[( )] "The assessor may be busy at the end of term."
****
The DPIA centres on risks to the people whose data is processed. Reputation, cost and workload are separate topics.
****

**Question 4.** Which design best follows minimisation for a public credential?

[( )] Show full legal name, date of birth, email and grade, to be safe
[( )] Add a public link to the full project report
[(X)] Show display name, credential title, criteria, issuer and issue date, and keep evidence private
[( )] Add the learner ID number so that the credential is unique
****
The credential states the claim. Items that serve no verifier need, and private evidence, stay out of the public view.
****

**Question 5.** A verifier needs to know that a badge is valid and issued by the academy. What is the best approach?

[( )] Publish the full learner record on a public page
[( )] Show the test score and trainer comment
[(X)] Present title, issuer and date with a status check, and keep scores and comments private
[( )] Send the learner's personal email to the verifier
****
Match the disclosure to the verifier's need. Existence, issuer and currency are enough.
****

**Question 6.** Which statement about expiry is accurate?

[( )] Expiry, public page end and issuer record retention are the same thing
[(X)] The validity of the claim, the end of the public page and the retention of the issuer's record are separate decisions
[( )] Expiry removes the credential from the earner's wallet automatically in every format
[( )] Expiry is only a design choice for colours
****
Each of the three has its own purpose and reason. Treating them as one leads to data kept for no purpose or claims that look current when they are not.
****

**Question 7.** Which status design reduces the risk that the issuer learns where an earner shows a credential?

[( )] A unique status URL per credential with full logging
[( )] A public page that lists the reason for each revocation
[(X)] A shared status list with no names, plus short log retention
[( )] A phone call to the earner each time
****
A shared list hides which entry a verifier read. Short log retention limits what can be learned over time.
****

**Question 8.** An AI tool flags a learner for suspected misconduct. Which DPIA entry is best?

[( )] The tool's flag leads to automatic revocation
[( )] The learner is told after the credential disappears
[(X)] A person reviews the flag before any outcome, the learner is told and can challenge, and the tool's data use is covered by the processor agreement
[( )] The flag is published to employers
****
Outcomes that affect the earner need human review and a route to challenge. The AI processor must also appear in the processor and transfer register.
****

**Question 9.** A hosted service stores learner data in the EEA, but its support team in another country can view records. What should the DPIA do?

[( )] Ignore it, because the data is stored in the EEA
[(X)] Record it as a possible transfer, name the mechanism and any extra measures, or plan an action
[( )] Delete the DPIA section on transfers
[( )] Publish the support team's names
****
Remote access can count as a transfer. Document the mechanism and measures, or create an action to find them out.
****

**Question 10.** Which processor agreement point deals directly with an AI tool provider using your data to improve its own models?

[( )] The provider's opening hours
[( )] The design of the provider's website
[(X)] A term that the provider processes data only on your documented instructions and does not use it for its own purposes
[( )] The number of languages the tool supports
****
Processing only on documented instructions, with no own-purpose use, is the core control. Where a provider uses data for its own purposes it acts as a controller for that use.
****

## Sources and further reading

Status as of November 2026; check before publishing.

- **Regulation (EU) 2016/679 (General Data Protection Regulation).** Official text on EUR-Lex, the legal database of the European Union. Read the provisions on data protection impact assessment, processors and transfers in the current consolidated text.
- **European Data Protection Board (EDPB).** Guidelines and opinions on data protection impact assessment, controllers and processors, and transfers, published on the EDPB website.
- **National data protection authorities.** Many publish DPIA templates, lists of processing that requires a DPIA, and guidance on education and employment. Use the authority responsible for your organisation.
- **European Commission, European Digital Identity Framework and EUDI Wallet.** Official pages and technical specifications (the Architecture and Reference Framework) published by the European Commission.
- **OpenID Foundation.** Specifications in the OpenID for Verifiable Credentials family (OpenID4VCI and OpenID4VP).
- **IETF.** The specification work on SD-JWT and SD-JWT-based verifiable credentials, published as drafts or RFCs in the IETF datatracker.
- **ISO/IEC 18013-5.** International standard for mobile driving licences (the basis for the mdoc credential format), published by ISO.
- **W3C.** The Verifiable Credentials Data Model and related recommendations.
- **ISO/IEC 27701.** Privacy information management extension to ISO/IEC 27001, published by ISO.
- **ICoBC Credentialing Skills Framework (ICSF).** Skill SECP "Security, privacy and data protection", published by ICoBC.
- **ICB-F10 Data Protection Basics for Credential Issuers.** The prerequisite course in the ICoBC Kursbibliothek.

<!-- VERIFY: Confirm the current titles, numbers and publication status of each listed standard and specification (including the EUDI Architecture and Reference Framework and any Digital Omnibus changes to data rules) before publishing. No URLs are given by design. -->

**Time-sensitive points.** GDPR and data protection law are established and stable; watch for changes under the Digital Omnibus. Wallet protocols and credential formats (OpenID4VC, SD-JWT VC, ISO mdoc) are emerging: specified for the EUDI Wallet, with tooling and education profiles still maturing. Rules on AI systems in education and employment are developing. Status as of November 2026; check before publishing.
