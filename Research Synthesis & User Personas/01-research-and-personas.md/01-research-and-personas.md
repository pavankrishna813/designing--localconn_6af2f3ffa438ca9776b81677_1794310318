# LocalConnect — Research foundation and proto-personas

Prepared 10 November 2026 • Group project working draft

**Evidence status:** No participant interviews, surveys or usability sessions have been conducted for this draft. The pain points come from the assignment brief; the personas and behavioural insights below are hypotheses. They must not be presented as validated findings. Names and scenarios are fictional. Bengaluru is a provisional design setting, not an inferred user location.

## Problem and scope

The assignment describes a clunky community-event experience with unclear navigation and outdated presentation. LocalConnect should let residents discover relevant nearby activities, understand cost and participation requirements, register, and retrieve the registration later.

Primary journey: discover → evaluate → register → retrieve. Initial scope is free, in-person events. Payments, messaging, organiser administration and social feeds are deferred to keep the core journey testable.

## Research questions

1. How do residents currently find local activities, and where does that process fail?
2. Which details determine whether someone attends: timing, travel, cost, accessibility, companions or organiser credibility?
3. What makes people abandon registration?
4. What information do people need after reserving a place?

## Research protocol ready to run

Recruit 5–6 adult residents across newcomers, busy residents and people who need clear access information. Include varied technical confidence. Use a 20-minute interview, with voluntary participation and permission before recording. Refer to participants as P01–P06; collect no unnecessary identifiers. Keep raw notes private and agree a deletion date with participants.

Interview prompts:

- Tell me about the last local event you considered attending. How did you find it?
- Walk me through how you decided whether to go. What information was missing?
- Show or describe your most recent registration experience. Where did you hesitate?
- How did you find the venue or retrieve your confirmation later?
- What would make an unfamiliar local event feel safe and worth your time?

Avoid leading questions such as “Would a map make this easier?” Record observed behaviour separately from interpretation. For each insight capture participant ID, paraphrase or permitted exact quote, context, counterevidence, confidence and design implication. Do not invent quotes or percentages.

## Assumption register

| ID | Hypothesis | Proposed response | Validation |
| --- | --- | --- | --- |
| H1 | Date and travel distance narrow choices early | Visible date, location and distance; editable filters | Ask residents to choose an event and observe filter use |
| H2 | Hidden costs and missing logistics reduce confidence | Show price, duration, venue, organiser and access details before registration | Ask participants to explain attendance requirements |
| H3 | Long forms interrupt intent | Short registration with field-level errors and preserved input | Observe task completion and error recovery |
| H4 | Unclear confirmation causes repeat registration | Explicit success state and persistent My events entry | Ask users to retrieve the reservation later |
| H5 | A map helps some users but is insufficient alone | Provide a complete readable list alternative | Test with varied visual and navigation preferences |

## Three proto-personas — assumptions, not research findings

### Ananya — newcomer seeking connection

Fictional 24-year-old who recently moved to the neighbourhood and uses a mobile phone confidently. Goal: find a welcoming weekend activity without travelling far. Assumed barriers: unfamiliar venues and uncertainty about attending alone. Needs: clear location, organiser identity, beginner suitability and a low-pressure registration. Scenario: find a free Saturday gardening event within a comfortable trip, check what to bring, and reserve one place. Validation: investigate how newcomers judge trust rather than assuming demographic characteristics determine behaviour.

### Ravi — resident with a constrained schedule

Fictional 38-year-old balancing work and family commitments. Goal: identify an activity that fits a specific available time. Assumed barriers: browsing irrelevant dates and unclear duration or age suitability. Needs: date/time filtering, end time, transparent price and eligibility. Scenario: compare two Saturday activities and save one before deciding. Validation: ask how actual residents coordinate attendance; do not assume everyone attends with children.

### Meera — resident who needs clear access information

Fictional 61-year-old who values readable interfaces and checks venue access before attending. Goal: confidently choose an accessible local activity. Assumed barriers: small text, icon-only controls and vague venue descriptions. Needs: readable labels, keyboard/screen-reader support, step-free access information and a clear way to ask the organiser. Scenario: confirm the venue entrance and seating arrangements before registering. Validation: recruit people with relevant access needs; age is not evidence of disability or digital skill.

## Hypothetical journey map

| Stage | User question | Potential friction (hypothesis) | Design response |
| --- | --- | --- | --- |
| Discover | What can I join nearby? | Irrelevant or stale results | Location/date context and clear empty state |
| Evaluate | Is this right for me? | Hidden logistics or eligibility | Practical details before the call to action |
| Register | What information is required? | Long form, unclear errors | Minimal labelled fields and retained values |
| Confirm | Do I have a place? | Ambiguous success | Event summary and reservation status |
| Attend | Where is my reservation? | Confirmation hard to retrieve | My events entry and cancellation information |

## Desk comparison — documented capabilities, not a hands-on audit

Reviewed 10 November 2026. Eventbrite's app help documents discovery with date/category/price filters and checking event time and location. Meetup's help documents event discovery through search and filters. These establish familiar interaction patterns; they do not prove LocalConnect users need them or establish either product's usability.

| Reference | Documented pattern | LocalConnect implication (design inference) |
| --- | --- | --- |
| [Eventbrite app help](https://www.eventbrite.com/help/en-gb/articles/783059/how-to-use-the-eventbrite-iphone-app/) | Filter discovery and check event details | Keep the minimum decision details visible |
| [Meetup: Finding an event](https://help.meetup.com/hc/en-us/articles/39235072484109-Finding-an-event) | Search and filtered event discovery | Use familiar search/filter language |

## Synthesis completion criteria

Replace hypotheses with evidence only after interviews. Attach anonymised notes and affinity groups; state sample limitations; update personas with observed motivations; link every priority design decision to evidence or clearly marked assumptions. Research deliverable remains provisional until then.
