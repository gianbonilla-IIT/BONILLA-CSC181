# Product Backlog

## Team Information

- Team name: Meridian  
- Project title: iitmaps: every office, one search away  
- Primary user group for the first release: MSU-IIT students, especially first years and student organization officers  
- Format: User stories with one use case

| Member | GitHub username | Personal CSC181 repository |
| :---- | :---- | :---- |
| Lex Ian G. Cabasag | codex-coderex | [Repository link](https://github.com/codex-coderex/csc181) |
| Michael S. Sumagui | michaelsumagui-create | [Repository link](https://github.com/michaelsumagui-create/CSC181) |
| Francis Cris P. Gerondio | franciscrisgerondio-a11y | [Repository link](https://github.com/franciscrisgerondio-a11y/CSC181_Gerondio_Submissions) |
| Gian Christian S. Bonilla | gianbonilla-IIT | [Repository link](https://github.com/gianbonilla-IIT/BONILLA-CSC181) |

## 1\. Interview Summary

We ran an online student survey, "Finding offices and rooms at MSU-IIT". It received 32 submissions. Two did not consent, one stopped after saying they have never needed to find an unfamiliar place, so 29 respondents completed it. Respondents are identified only by group code. No staff, administrators, or visitors responded.

| Code | Stakeholder role | Date | Method | Interviewer(s) |
| :---- | :---- | :---- | :---- | :---- |
| V1 | Students not in a student organization (n=11 of 29 completed) | October 2026 | Online survey | Team Meridian |
| V2 | Student organization officers and members (n=18 of 29 completed: 10 officers, 8 members) | October 2026 | Online survey | Team Meridian |

## 2\. From Interview Notes to Needs

| ID | Source | What we heard or saw | Underlying need | Requirement idea | Type |
| :---- | :---- | :---- | :---- | :---- | :---- |
| F1 | V1, V2 | 16 of 29 asked a classmate or org mate, 15 walked around, 9 asked staff, 7 asked a guard. Only 4 read a posted floor plan or directory. | Find an office without relying on other people. | Searchable directory where a user types an office name and gets redirected to its location in a 2d map. | F |
| F2 | V1, V2 | 14 of 29 went to the wrong place first, and 14 felt frustrated or stressed. | Be sure of the right building, floor, and room before walking. | Show the building, floor, and room highlighted on a floor plan. | F |
| F3 | V1, V2 | 20 of 23 would use search by office name and 17 of 23 search by room number. One respondent asked for keywords in each office. | Reach a known destination with as few clicks or taps as possible. | Search by office name and by room number, with optional keywords. | F |
| F4 | V1, V2 | 19 of 23 would use browsing by building and floor. 13 of 17 who suggested improvements asked for a map. | See which rooms or offices are on a floor when the exact name of the room or office is not known. | Allow users to browse the directory from campus view (showing buildings) to floor plan view (showing rooms). | F |
| F5 | V2 | Of 16 who run errands, 9 visit 2 to 3 offices per trip and 11 spend at least half the trip finding offices. 15 of 23 would use office hours. 1 respondent missed a deadline or office hours. | Know whether an office is open before visiting to avoid arriving when the office is closed. | Show office hours in each room (when applicable). | F |
| F6 | V1, V2 | If sent to a wrong room, 23 of 29 would report it, 16 would double-check, and 1 would stop using the directory. Respondents asked for up to date information. | Keep the map accurate and trusted. | Display the last verified date on the footer of each map. Moreover, provide a report link for every listing. | F |
| F7 | V1, V2 | 5 of 21 who gave a reason do not want to open another app or site. One respondent asked that it be easy for guests. One suggested a link from MyIIT. | Use the features with no additional setup cost. | Web-based directory with no account, light pages, loading within 3 seconds, usable on a phone. | Q |
| F8 | V1, V2 | 2 respondents asked for offline access. One wrote that it should be usable without the internet. | Find rooms when the connection is weak or missing. | Upon first access to the web app, the whole directory is saved on the device, so offline use is possible afterwards.   | Q |
| F9 | V1, V2 | The Administrative Building was named 5 times, CASS and CSM 4 times each. | Cover the places where people actually get lost. | Pilot with the Administrative Building and CASS. | C |
| F10 | V2 | These elements were also requested aside from location information: contact information, room booking process per office, office heads with photos, facility availability, trash bin locations, real-time GPS. | Extra information around the room element beyond its location. | Display the office head and contact details on each office listing (when the office has them). | F |

### Assumption log

| ID | Assumption | Risk if wrong (High/Medium/Low) | How we will check it |
| :---- | :---- | :---- | :---- |
| A1 | Existing campus maps are accurate enough to serve as a starting layout. | High | Compare the maps with a sample of rooms on every floor of the Administrative Building and CASS during on site visits. |
| A2 | Office locations stay stable during the semester. | High | Ask office staff about planned moves and record a last verified date per entry. |
| A3 | The administration allows mapping of the Administrative Building. | Medium | Ask the administration which areas must not be mapped before collecting data. |
| A4 | Office staff and visitors have needs similar to the students we surveyed. | Medium | Interview office staff and visitors. |
| A5 | Stated intent to use (average 4.7 out of 5\) turns into real use. | Medium | Measure real use and timed tasks during prototype testing. |
| A6 | Offices agree to have their office head's name and contact details published. | Medium | Ask each office for consent before adding its details to a listing. |

## 3\. User Stories

| ID | User story | Source finding(s) | Epic | INVEST check |
| :---- | :---- | :---- | :---- | :---- |
| US-01 | As a student, I want to search for an office by name, so that I can reach it without asking other people. | F1, F3 | Find an office | Yes |
| US-02 | As a student, I want to search by room number, so that I can find a room when I only know its number. | F3 | Find an office | Yes |
| US-03 | As a student, I want to see the searched room highlighted on a floor plan, so that I do not go to the wrong place first. | F2 | See where it is | Yes |
| US-04 | As a student, I want to switch between floors and buildings on the floor plan, so that I can confirm the right floor and building before I walk there.  | F4 | See where it is | Yes |
| US-05 | As an organization officer, I want to browse offices by building and floor, so that I can plan visits to several offices in one trip. | F4, F5 | See where it is | Yes |
| US-06 | As an organization officer, I want to see the office hours of each office, so that I do not arrive when the office is closed. | F5 | Plan an errand | Yes |
| US-07 | As a student or organization officer, I want to report wrong or outdated information through a link, so that the map gets corrected. | F6 | Trust the data | Yes |
| US-08 | As a guest or visitor, I want to use the directory without an account, so that I can start searching right away. | F7 | Access | Yes |
| US-09 | As a student walking between buildings, I want search results to appear within 3 seconds on my phone, so that I get an answer without stopping. | F7 | Access | Yes |
| US-10 | As a student with a weak connection, I want to reopen the floor plans I viewed before without the internet, so that I don’t get inconvenienced by the lack of internet. | F8 | Access | Yes |
| US-11 | As a student, I want to see when a map was last verified, so that I can judge whether to trust it. | F6 | Trust the data | Yes |
| US-12 | As an organization officer, I want to see relevant office details, such as the list of staff and contact info (when applicable) on each room, so that I can plan my visit without making unnecessary trips.  | F10 | Plan an errand | Yes |
| US-13 | As a student, I want to search offices by keyword, so that I can find an office when I do not know its exact name. | F3 | Find an office | Yes |

### Epics and how we split them

| Epic | Split into | How we split it |
| :---- | :---- | :---- |
| Find an office | US-01, US-02, US-13 | By data type: office name, room number, keyword. |
| See where it is | US-03, US-04, US-05 | By workflow step: view the room, change floor or building, browse by floor. |
| Plan an errand | US-06, US-12 | By business rule: office hours first, list of staff, and contact information. |
| Trust the data | US-07, US-11 | By workflow step: let users report, then show when the entry was verified. |
| Access | US-08, US-09, US-10 | By business rule: no account first, response time second, offline last. |

### Stories we rewrote

1. Before: As a student, I want a campus map, so that I can find places. After: US-01, US-02, US-03, and US-04. Reason: The original was too large and not testable (missing Small and Testable). Survey answers asked for maps, but the useful parts are search, a highlighted floor plan, and floor switching.  
2. Before: As a user, I want the directory to be fast, work offline, and need no account. After: US-08, US-09, and US-10. Reason: Three separate needs in one story (missing Small and Independent). Offline use is a stretch goal and should not block the other two.

## 4\. Acceptance Criteria

Example values below (office names, room numbers) are sample data for testing, not real listings.

### US-01: Search an office by name

Acceptance criteria:

- [ ] Typing at least 3 characters of an office name shows the matching offices in a list.  
- [ ] Matching ignores uppercase and lowercase.  
- [ ] Each result shows the office name, building, and floor.  
- [ ] (unhappy) If no office matches, the page shows "No office found" and a link to browse by building and floor.

Scenario 1: Normal case

```
Given the directory has "Sample Office" in the Administrative Building, 2nd floor, room 201
When the user types "sample" in the search box
Then the results list shows "Sample Office, Administrative Building, 2nd floor"
```

Scenario 2: Unhappy path

```
Given the directory has no office named "Zzz Office"
When the user types "Zzz Office" in the search box
Then the page shows "No office found" and a link to browse by building and floor
```

### US-02: Search by room number

Acceptance criteria:

- [ ] Entering a room number that exists in a pilot building shows that room's listing.  
- [ ] The result shows the building, floor, and the office assigned to the room.  
- [ ] The search accepts the number with or without spaces around it.  
- [ ] (unhappy) A room number that is not in the data shows "Room not found".

Scenario 1: Normal case

```
Given room 201 in the Administrative Building is assigned to "Sample Office"
When the user enters "201" in the room number search
Then the page shows "Sample Office, Administrative Building, 2nd floor, room 201"
```

Scenario 2: Unhappy path

```
Given no room 999 exists in the data
When the user enters "999" in the room number search
Then the page shows "Room not found"
```

### US-03: View the highlighted floor plan

Acceptance criteria:

- [ ] Opening a listing shows the floor plan of its floor with its room highlighted.  
- [ ] The building name and floor number appear above the plan.  
- [ ] The highlighted room differs from other rooms by both an outline and a fill color.  
- [ ] (unhappy) If the plan for that floor is missing, the page shows the building, floor, and room number as text with the report link.

Scenario 1: Normal case

```
Given "Sample Office" is in room 201, Administrative Building, 2nd floor, and the 2nd floor plan exists
When the user opens the "Sample Office" listing
Then the 2nd floor plan is shown with room 201 outlined and filled
```

Scenario 2: Unhappy path

```
Given the plan for CASS 3rd floor is not in the data and "Sample Lab" is listed there in room 305
When the user opens the "Sample Lab" listing
Then the page shows "CASS, 3rd floor, room 305" as text and a report link
```

### US-04: Switch floors and buildings

Acceptance criteria:

- [ ] The floor selector lists every floor that has plan data for the current building.  
- [ ] Selecting a floor shows that floor's plan within the same page.  
- [ ] The building selector lists the Administrative Building and CASS.  
- [ ] (unhappy) A floor without data appears disabled with the label "No plan yet".

Scenario 1: Normal case

```
Given the user is viewing the Administrative Building 2nd floor plan
When the user selects the 3rd floor
Then the 3rd floor plan of the Administrative Building is shown
```

Scenario 2: Unhappy path

```
Given the 4th floor of CASS has no plan data
When the user opens the CASS floor selector
Then the 4th floor appears disabled with the label "No plan yet"
```

### US-05: Browse offices by building and floor

Acceptance criteria:

- [ ] The campus view lists the Administrative Building and CASS, and selecting a building opens its floor list.  
- [ ] Selecting a building and a floor lists all offices on that floor in alphabetical order.  
- [ ] Each entry shows the office name and room number.  
- [ ] Selecting an entry opens its listing.  
- [ ] (unhappy) A floor with no listed offices shows "No offices listed for this floor".

Scenario 1: Normal case

```
Given the Administrative Building 2nd floor has "Sample Office" (room 201) and "Another Office" (room 202)
When the user selects Administrative Building and 2nd floor
Then the list shows "Another Office, 202" followed by "Sample Office, 201"
```

Scenario 2: Unhappy path

```
Given CASS 1st floor has no offices in the data
When the user selects CASS and 1st floor
Then the page shows "No offices listed for this floor"
```

### US-06: See office hours

Acceptance criteria:

- [ ] Each listing shows office hours as days and times.  
- [ ] Times use the 12 hour format with AM or PM.  
- [ ] The hours appear on the listing page without extra clicks.  
- [ ] (unhappy) If office hours are not set, the listing shows "Hours not specified". 

### US-07: Report wrong or outdated information

Acceptance criteria:

- [ ] Every listing has a "Report wrong or outdated information" link.  
- [ ] The report form accepts a description of up to 300 characters and needs no account.  
- [ ] After submitting, the page shows a confirmation message.  
- [ ] (unhappy) Submitting an empty description shows an error and sends nothing.

### US-08: Use the directory without an account

Acceptance criteria:

- [ ] Opening the site address shows the search page with no login screen.  
- [ ] Search, browse, and floor plan features work for a user who has not signed in.  
- [ ] No page asks for a name, email, or password.  
- [ ] (unhappy) If the browser blocks cookies, search and browse still work.

Scenario 1: Normal case

```
Given a new visitor on a phone who has never opened the site
When the visitor opens the site address
Then the search box is shown and no login prompt appears
```

Scenario 2: Unhappy path

```
Given the visitor's browser blocks cookies
When the visitor searches for "sample"
Then the results list is shown as usual
```

### US-09: Load within 3 seconds on a phone

Acceptance criteria:

- [ ] The search page loads within 3 seconds on a simulated 4G connection.  
- [ ] The layout fits a 360 pixel wide screen with no horizontal scrolling.  
- [ ] The initial page download is at most 1 MB.  
- [ ] (unhappy) If loading takes longer than 5 seconds, a loading message is shown.

### US-10: Save the directory and use it offline

Acceptance criteria:

- [ ] After the search page has loaded, the system downloads all floor plans and listings of the Administrative Building and CASS to the device.  
- [ ] With the network turned off, search by office name and by room number, browsing by building and floor, and opening floor plans work from the saved directory.  
- [ ] The download does not delay search results beyond the 3 seconds in US-09.  
- [ ] The page shows an "Offline" label when the network is unavailable.  
- [ ] The page shows "Saved for offline use" when the download finishes.  
- [ ] (unhappy) If the connection drops before the download finishes, the page shows "Directory not fully saved" and resumes the download on the next visit with a connection.  
- [ ] (unhappy) If the directory was never saved and the network is off, the page shows "Open iitmaps once with internet to use it offline".

### US-11: See the last verified date

Acceptance criteria:

- [ ] Each floor plan shows "Last verified" with a date in YYYY-MM-DD format in its footer.  
- [ ] The date shown equals the verified date stored for that floor plan in the data.  
- [ ] After the stored date is updated and the page is reloaded, the footer shows the new date.  
- [ ] (unhappy) A floor plan that was never verified shows "Not yet verified" in its footer.

### US-12: View staff and contact information

Acceptance criteria:

- [ ] A listing shows the list of all staff and their contact information (when applicable).  
- [ ] All available details appear directly on the listing page without extra clicks.  
- [ ] (unhappy) If the selected room is not an office, the office details section is hidden entirely.  
- [ ] (unhappy) If no staff and contact information are stored, the listing shows "No staff information listed".

### US-13: Search by keyword

Acceptance criteria:

- [ ] Each office can store one or more keywords.  
- [ ] Searching for a keyword returns every office that has it.  
- [ ] Name matches appear above keyword matches in the results.  
- [ ] (unhappy) A keyword with no match shows "No office found".

## 5\. Quality Requirements and Constraints (EARS)

| ID | Requirement | EARS pattern | Type | Source | Number agreed with |
| :---- | :---- | :---- | :---- | :---- | :---- |
| NFR-01 | While the device has no network connection after the directory has been saved, the system shall display the saved floor plans and listings.  | State-driven | Quality | F8 | N/A |
| NFR-02 | When a user submits a search, the system shall show results within 3 seconds on a simulated 4G connection. | Event-driven | Quality | F7 | N/A |
| NFR-03 | The system shall allow search, browsing, and floor plan viewing without an account. | Ubiquitous | Constraint | F7 | N/A |
| NFR-04 | When a listing is displayed, the system shall show the date the listing was last verified. | Event-driven | Quality | F6 | N/A |
| NFR-05 | The system shall include floor plan data only for the Administrative Building and CASS in the first release. | Ubiquitous | Constraint | F9 | N/A |
|  |  |  |  |  |  |

## 6\. Use Case

### Use-case diagram

\!\[Use-Case Diagram\](backlog-images/use-case-diagram.png) 

### UC-01: Find an office and see where it is

| Field | Description |
| :---- | :---- |
| Primary actor | Student, organization officer, or guest |
| Precondition | The user has opened the iitmaps site in a browser, and data for the Administrative Building and CASS is loaded. |
| Main success scenario | 1\. The user enters an office name or room number in the search box.    2\. The system lists the matching offices.     3\. The user selects an office.    4\. The system shows the building, floor, and room highlighted on the floor plan, with the office hours.    5\. The user switches floors on the plan if needed. |
| Extensions | 1a. The device has no network, and the directory was saved earlier (Release 2): the system searches the saved directory and shows an "Offline" label. 2a. No office matches: the system shows "No office found" and a link to browse by building and floor.    2b. Several offices match: the system lists each with its building and floor, and the user picks one.    4a. The floor plan is missing: the system shows the building, floor, and room number as text with the report link. |
| Postcondition | The user knows the building, floor, and room of the office. |
| Stories covered | US-01, US-02, US-03, US-04, US-06, US-10 |

## 7\. Story Map

|  | Open the directory | Find the office | See where it is | Check details and report |
| :---- | :---- | :---- | :---- | :---- |
| **Release 1 (MVP)** | US-08 | US-01, US-02, US-05 | US-03, US-04 | US-06, US-07 |
| **Release 2** | US-09, US-10 | US-13 |  | US-11 |
| **Later** |  | US-12 |  |  |

## 8\. The Ordered Backlog

| Rank | Story | MoSCoW | Size (S/M/L) | Value / effort quadrant | Sprint |
| :---- | :---- | :---- | :---- | :---- | :---- |
| 1 | US-01 Search an office by name | Must | S | Quick win | Sprint 1 |
| 2 | US-02 Search by room number | Must | S | Quick win | Sprint 1 |
| 3 | US-08 Use without an account | Must | S | Quick win | Sprint 1 |
| 4 | US-03 View the highlighted floor plan | Must | M | Big bet | Sprint 1 |
| 5 | US-05 Browse by building and floor | Must | M | Big bet | Sprint 2 |
| 6 | US-04 Switch floors and buildings | Must | M | Big bet | Sprint 2 |
| 7 | US-06 See office hours | Should | S | Quick win | Sprint 2 |
| 8 | US-07 Report wrong information | Should | S | Quick win | Sprint 2 |
| 9 | US-11 See the last verified date | Should | S | Quick win | Later |
| 10 | US-09 Load within 3 seconds on a phone | Should | M | Big Bet | Later |
| 11 | US-13 Search by keyword | Could | S | Filler | Later |
| 12 | US-10 Save the directory and use it offline | Could | L | Time Sink | Later |
| 13 | US-12  View office details and staff info  | Won't | M | Time Sink | Not this time |

### How we ordered it

Search by name and room number are first because they were the most chosen features (20 and 17 of 23), and they are the shortest path to a known destination. The highlighted floor plan comes next because it answers the wrong turn problem that 14 of 29 respondents reported, and it depends on the floor plan data, which is our biggest risk. Browsing and floor switching depend on that same data, so they follow. Office hours and the report link are “should” items that complete the Release 1 path. Offline use is large and was requested by only 2 respondents, and the office and staff information needs data we do not have yet, so both are last. “Won't” stories are kept, not deleted.

### Capacity check

| Question | Answer |
| :---- | :---- |
| How many Must-have stories, and their total size? | 6 stories: 3 small (US-01, US-02, US-08) and 3 medium (US-03, US-04, US-05). |
| Do the Must-haves fit in about 60% of our time for two sprints? | Yes, by our estimate. The three small stories fit in Sprint 1 with US-03, and the other two medium stories fit in Sprint 2 with the Should stories. The team still needs to confirm this estimate. |
| Do the Release 1 stories form one complete path through the core workflow? | Yes. Release 1 covers open, find, see where it is, and check details. |
| Are all L-sized Must-have stories split? | Yes. There are no L-sized Must-have stories. The only L story (US-10) is a Could. |

## 9\. Definition of Done

- [ ] Every acceptance criterion of the story passes in a manual test on a phone sized browser and a desktop browser.  
- [ ] Another team member reviewed the code and it was merged into the main branch of the team repository.  
- [ ] Any floor plan or listing data used by the story has a last verified date.  
- [ ] The story was demonstrated to the team at the end of the sprint with no open defects.

## 10\. Traceability Table

| Story | Problem or goal it addresses | Source finding(s) | Test cases (Week 9\) |
| :---- | :---- | :---- | :---- |
| US-01 | Find an office without asking other people. | F1, F3 |  |
| US-02 | Reach a room when only the room number is known. | F3 |  |
| US-03 | Avoid going to the wrong place first. | F2 |  |
| US-04 | Check the right floor and building before walking. | F4 |  |
| US-05 | Plan visits to several offices in one trip. | F4, F5 |  |
| US-08 | Use the directory with no setup cost. | F7 |  |

Gaps found: None.

## 11\. Validation

### Team review

| Problem found | Story or requirement | How we fixed it |
| :---- | :---- | :---- |
| The previous US-09 expresses a rigid system-wide performance metric as a feature story. (fails *Negotiable*, *Estimable*, & *Small*) | US-09 (F7) | Rephrased it so it describes a clear, actionable user feature focused on asset optimization, while also keeping the 3-second target as testable acceptance criteria. |
| The story used overly broad terms ("lightweight information") and an abstract benefit ("so that I will be more knowledgeable"), leaving developers without clear data fields to build and QA without testable acceptance criteria. (fails *Estimable* & *Testable*) | US-12 (F5, F10) | Replaced vague phrasing with concrete, verifiable fields (staff list, and contact info) on room listings, and re-aligned the user goal to an actionable outcome (planning visits without unnecessary trips). |
| The role "user" hid who the story is for (common mistake, slide 31). | US-07 (F6) | Changed the role to "student or guest". |
| "Check the right path" was unclear because the first release has no route feature (fails Testable). | US-04 (F4) | Reworded the benefit to "check the right floor before I walk". |

### Stakeholder walk-through

| Stakeholder | Date | What they said | What we changed |
| :---- | :---- | :---- | :---- |
| V2 \- Organization Officer | 2026-11-09 | “The idea is good, especially the idea to make it so that each floor shows a 2d floor plan and the search results make it so the name of the office in the floor plan lights up” | None. They like the idea. |
| V1 \- Student not in an Organization | 2026-11-09 | “The idea is really great. It would be even greater if you can apply live routing” | None. Live routing is out of our scope. |
| V1 \- Student not in an Organization | 2026-11-09 | “It is quite good. I like the idea of being able to use it offline, making the loading time fast, being able to report outdated places, and seeing when was the last time the location was verified.” | None. They like the idea. |

## 12\. Open Questions for Sprint 1

1. Can we obtain official or more detailed floor plans for the Administrative Building and CASS from the colleges or administration?  
2. How long will it take the team to collect and verify the room data for every floor of the Administrative Building and CASS, and can it be finished early enough to leave time for building and testing?  
3. What do office staff, administrators, and visitors think about listing offices (privacy, accuracy, security)?

## 13\. Member Contribution Record

| Member | Interviews or analysis | Stories, criteria, or use case | Review or validation |
| :---- | :---- | :---- | :---- |
| Lex Ian G. Cabasag | Created the initial feasibility survey and posted it to collect responses  | Reviewed and revised stories, criteria, and use cases | Reviewed multiple sections of the backlog, suggested tweaks, and raised questions for the team to check and resolve. |
| Michael S. Sumagui | Checked the survey results against the findings in Section 2\. | Fixed and updated some user stories and acceptance criteria (Sections 3 and 4).  | Reviewed multiple sections of the backlog, suggested edits, and raised questions so that the team can check and resolve. |
| Francis Cris P. Gerondio | Reviewed the feasibility survey and disseminated it to collect responses. Analyzed results | Drafted and revised stories, criteria, and use cases. | Reviewed and validated multiple sections of the backlog, suggested edits, and raised questions so that the team can check and resolve. |
| Gian Christian S. Bonilla | reviewed and analyzed results to start working in the backlog | reviewed the draft revised some contents of sec.2;  performed *INVEST* check on drafted user stories in sec.3 | corrected affected elements from the revisions (sec.4, sec.8, sec.10) drafted *INVEST* check validation (sec.11) |

## 14\. References

1. Week 3 and Week 4 lecture slides, CSC181.  
2. Team Meridian, "Finding offices and rooms at MSU-IIT" student survey, 32 submissions (30 consenting, 29 completed), October 2026\. Responses are kept in the team's survey sheet.  
3. Team Meridian, Team Brainstorming and Preliminary Project Proposal (iitmaps).

## 15\. Team AI Use Declaration

Select one option:

- [ ] No generative AI tools were used by any member in preparing this submission.  
- [x] One or more members used generative AI tools. Details are provided below.

| Member who used AI | Tool | Purpose and sections assisted | How output was checked or revised |
| :---- | :---- | :---- | :---- |
| Gian Christian S. Bonilla | Gemini (3.6 Flash) | Aside from the team performing the INVEST check, AI  was also used to further add insights on top of ours. | Its output was compared to our existing analysis. We deemed it was not always correct. For example, it failed some stories that were deemed passable. However, there were also some useful insights that influenced the revisions. |
| Francis Cris P. Gerondio | Claude (Anthropic) | Checked the team's draft against the Week 4 slides and the submission checklist, with suggestions to revise the product backlog from the team's survey results and project proposal. | The output was compared with the survey results, the project proposal, and the Week 4 slides. |

### Main prompts or interaction summary

Prompted by Gian Bonilla to Gemini:  
*“Could you do a comprehensive review on every aspect of the INVEST framework on every user story?”*

Prompted by Francis Cris Gerondio to Claude:   
*“This is the template of our backlog with existing drafts. Tell me what I can or need to add or changes I need to do if you compare the draft with the interview logs (attached file).”*

*“This is the current state of our product backlog, as you can see there are some changes but not much. I want you to take into account the changes. Then verify the contents of the file using the material I sent. Tell me what I can or need to add or changes I need to do for the file.”*

We acknowledge that AI-generated suggestions are not evidence of actual stakeholder interviews, feedback, or verified user needs. Every finding in Section 2 and every walk-through in Section 11 comes from a real person we spoke to or observed. We remain responsible for the accuracy and explainability of this submission.

## 16\. Team Confirmation

We confirm that this document reflects our team's agreed-upon product backlog. All members listed below reviewed the final version, and each member will upload the same Markdown file to their personal CSC181 repository.

| Member | Reviewed final version |
| :---- | :---- |
| Lex Ian G. Cabasag | Yes |
| Michael S. Sumagui | Yes |
| Francis Cris P. Gerondio | Yes |
| Gian Christian S. Bonilla | Yes |

## Submission Checklist

- [x] Interviews cover at least two stakeholder groups, with sources coded and no personal information.  
- [x] The needs table has at least 8 findings, each labelled F, Q, or C.  
- [x] Assumptions are recorded separately from evidence.  
- [x] There are 10 to 15 user stories, each with a real role, a "so that", and at least one finding.  
- [x] Epics are split, and at least two rewrites are recorded.  
- [x] Every story has at least 3 acceptance criteria, including an unhappy path, with no weak words.  
- [x] Every Must-have story has at least 2 Given–When–Then scenarios.  
- [x] At least 3 quality requirements or constraints use EARS patterns.  
- [x] One use case has a diagram, a main success scenario, and at least 2 extensions.  
- [x] The story map has a Release 1 line that crosses every journey step.  
- [x] Every story has a MoSCoW label and a size, and the backlog is in one order with no ties.  
- [x] Must-haves fit in about 60% of capacity. Won't-have stories are kept, not deleted.  
- [x] A Definition of Done is included.  
- [x] The traceability table covers every Must-have story.  
- [x] The team review and the stakeholder walk-through are recorded.  
- [x] Contributions, references, and AI use are declared.  
- [x] All members reviewed the same final document.  
- [x] Each member saved the file as `activities/product-backlog.md`, with images in `activities/backlog-images/`.  
- [x] Each member committed and pushed their copy to their personal repository.  
- [x] Each member submitted their own GitHub file link through MOLE before November 11, 2026 23:59:59.