# MediLingo

**An AI receptionist prototype that lets patients book medical appointments by text, ASL video, or in their own language, with no phone call needed.**

**Live demo:** https://ksusanto14.github.io/MediLingo/ *(available once GitHub Pages is turned on)*

MediLingo was built for an AI in Healthcare group project in *Management Principles and Practice* at Bryant University


---

## The problem

Most US medical practices book appointments mainly by phone. That shuts out patients who are deaf, hard of hearing, or speech-disabled. It also makes booking harder for people with language barriers. Research shows these patients are often hung up on or turned away, and many end up delaying or avoiding care. Federal law already requires providers to communicate effectively with patients with disabilities. The phone-based front desk keeps falling short of that.

## The solution

MediLingo is a receptionist patients can reach through text chat, ASL video, or their preferred language. It:

- finds out the reason for the visit
- offers open times and books the appointment directly into the provider's calendar
- asks about accessibility needs, such as an ASL interpreter, a video interpreter, live captions, or a spoken-language interpreter, and records them so the office is ready
- hands the conversation to front-desk staff when a request is urgent or unclear, or when the patient asks for a person

## What's in the app

The app has three tabs:

| Tab | Who it's for | What it does |
|---|---|---|
| **Book a visit** | Patients | A guided chat in English, Spanish or Portuguese, with a step-by-step progress bar, a live appointment summary card, a Back button, a Staff button, and a Larger text option |
| **Front desk** | Clinic staff | The weekly provider calendar with accommodation badges, a queue of patients waiting for staff (urgent messages flagged in red), an interpreter prep list, and a review button to mark each booking correct or needing a fix |
| **Dashboard** | Practice managers | Weekly bookings by channel, booking accuracy against a 95% goal, accommodations requested, languages used, reasons chats went to staff, and how full each provider's week is, with a 4 or 8 week filter and a table view |

## Try it

Open `index.html` in any web browser. There's nothing to install. Everything is in that one file.

A quick demo script:

1. On **Book a visit**, choose a visit type, a time, and an accommodation (for example, live captions), then enter a name and an email and tap **Book it**.
2. Open **Front desk** to see the new appointment highlighted on the calendar and added to the interpreter prep list.
3. Go back and type *"I have chest pain"*. MediLingo tells the patient to call or text 911 and flags the chat as urgent for staff.
4. On **Front desk**, select the new booking and mark it **Booked correctly** or **Needs a fix**.
5. Open **Dashboard** to see this week's numbers update.

## Prototype limitations

- **The chat follows a script.** It recognizes keywords and moves through set steps; it is not connected to a live AI model.
- **ASL recognition is simulated.** Patients can upload a video clip, then pick the phrase they signed.
- **The data is made up.** Riverbend Family Health and its providers are fictional. Calendar entries marked "sample" and all past weeks on the Dashboard are sample data.
- **Nothing is saved or sent.** No real messages, emails or texts are sent, and bookings reset when the page reloads.

A real version would also need strong privacy and security protections for patient information, integration with the practice's scheduling system, and ongoing accuracy monitoring. These are the same risks covered in our project paper.

## References

Blomstrand, S. M., Stark, C. L., McCarty, C. A., & Greminger, A. (2024). Exploring d/Deaf community perspectives regarding inclusive/accessible healthcare. *Journal of Regional Medical Campuses, 7*(2), Article 5570. https://doi.org/10.24926/jrmc.v7i2.5570

Boise State University. (2021, December 21). *Graduate uncovers inequities in access to health care for people who are deaf*. Boise State News. https://www.boisestate.edu/news/2021/12/21/graduate-uncovers-inequities-in-access-to-health-care-for-people-who-are-deaf/

Cohen, H. S., Della Santina, C. C., Dobie, R. A., Duffy, V. B., Hoffman, H. J., Losonczy, K. G., Rice, M. L., & Themann, C. L. (2019, February 9–13). *Burden of ear, nose and throat – voice, speech and language disorders based on United States health surveys, 2011–2016* [Conference abstract]. 42nd Midwinter Research Meeting of the Association for Research in Otolaryngology, Baltimore, MD, United States. https://stacks.cdc.gov/view/cdc/224668

Haas, M., & Mortensen, M. (2016, June). The secrets of great teamwork. *Harvard Business Review*, 70–76.

Haeder, S. F., & Xu, W. Y. (2025). What methods do patients use to schedule medical appointments? *Health Affairs Scholar, 3*(4), qxaf077. https://doi.org/10.1093/haschl/qxaf077

Nair, M., Svedberg, P., Larsson, I., & Nygren, J. M. (2024). A comprehensive overview of barriers and strategies for AI implementation in healthcare: Mixed-method design. *PLOS ONE, 19*(7), e0305949. https://doi.org/10.1371/journal.pone.0305949

National Institute on Deafness and Other Communication Disorders. (2024, September 20). *Quick statistics about hearing, balance, & dizziness*. U.S. Department of Health and Human Services, National Institutes of Health. https://www.nidcd.nih.gov/health/statistics/quick-statistics-hearing

Nondiscrimination in Health Programs and Activities, 89 Fed. Reg. 37522 (May 6, 2024) (to be codified at 45 C.F.R. pt. 92).

Parmar, B., Henshaw, H., Howe, S., Dickinson, A. M., Rolfe, C., Le Mere, P., Blondiaux-Ding, E., Musker, Z., & Stevenson, R. (2025). "I always feel like I'm the first deaf person they have ever met:" Deaf awareness, accessibility and communication in the United Kingdom's National Health Service (NHS): How can we do better? *PLOS ONE, 20*(5), e0322850. https://doi.org/10.1371/journal.pone.0322850

Ruiz Mejia, J. M., & Rawat, D. B. (2025). MedScrubCrew: A medical multi-agent framework for automating appointment scheduling based on patient-provider profile resource matching. *Healthcare, 13*(14), Article 1649. https://doi.org/10.3390/healthcare13141649

U.S. Department of Health and Human Services. (2024, June 4). *HHS Office for Civil Rights takes action to ensure access to care for patients who are deaf or hard of hearing* [Press release]. https://www.hhs.gov/about/news/2024/06/04/hhs-office-civil-rights-takes-action-ensure-access-care-patients-who-are-deaf-hard-hearing.html

Wood, K. V., Frings, D., Flood, C., & Thomas, N. (2025). Artificial intelligence machine learning-driven outpatient appointment management: A qualitative study on acceptability. *Digital Health, 11*, 1–15. https://doi.org/10.1177/20552076251321016
