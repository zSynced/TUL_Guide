# TUL Student Onboarding App — Functionalities & Use Cases

## [Website access](https://zsynced.github.io/TUL_Guide/)

## Target User

**First-year students at the Technical University of Łódź (TUL).**  
The app is designed specifically for new students navigating the beginning of their university journey — from completing enrollment paperwork to finding their first classroom.

---

## User Registration & Authentication

New students create an account using their email address and a password of their choice. Registration does not require a university-issued email, though students may choose to use their TUL SPE address (`albumNumber@edu.p.lodz.pl`).

Once logged in, the session is persisted — users stay signed in across visits so that checklist progress, profile details, and preferences are saved and restored automatically without needing to log in each time.

**Registration flow:**
1. Student opens the app for the first time and is prompted to create an account
2. Student enters their email address and chooses a password
3. An account is created and the student is logged in
4. On future visits, the session is restored automatically (no re-login required unless the user explicitly logs out)

**Password management:**
- Students can change their password from the Profile page
- Password must be at least 8 characters and confirmed before saving

**What is persisted per account:**
- Full name, email, and faculty selection
- Checklist step completion status
- Any future preferences or settings

---

## 1. Post-Admissions Onboarding (Checklist)

A guided checklist helping students complete all required steps before and at the start of university.

### Features
- 7 pre-defined onboarding steps, each with a title, short meta description, and expandable detail panel
- Tap to expand/collapse individual steps for more information
- Checkbox to mark each step as done, with visual strikethrough on completion
- Progress bar and percentage tracker updating in real time
- Tip banner reminding students to activate their TUL email (SPE)

### Checklist Steps
1. Submit enrollment documents
2. Take the matriculation oath
3. Activate TUL email (SPE) at poczta.p.lodz.pl
4. Log into WebDziekanat & WIKAMP
5. Get student ID card (ELS)
6. Explore the TUL campus
7. Orientation Days

### Use Cases

**UC-1.1 — Tracking onboarding progress**  
A student has just been accepted to TUL and opens the app. They see the checklist on the home screen with 0% progress. They read through the steps and mark "Submit enrollment documents" as done after visiting the Recruitment Office. The progress bar updates to 14%. On their next visit, the app loads with their saved progress — the step remains checked.

**UC-1.2 — Getting guidance on a specific step**  
A student is unsure what the ELS student ID card is. They tap the step to expand it and read that it grants library access and public transport discounts, and that they need to submit a photo via WebDziekanat. They follow the instructions and mark the step complete.

**UC-1.3 — Returning after a break**  
A student completed 3 steps last week. They open the app again and their checklist is exactly as they left it — no need to re-check anything or log in again.

---

## 2. Campus Navigation (Map)

An interactive campus map to help students locate buildings and key university facilities.

### Features
- Embedded interactive map via mapa.p.lodz.pl displayed inside the app
- "Open full" link to launch the full map in a browser
- Quick-access list of key campus locations with icons and addresses

### Key Locations Listed
- Main Building (B3) — ul. Ks. I. Skorupki 10/12
- Main Library — ul. Wólczańska 221
- Student Canteen — al. Politechniki 8
- Student Health Centre — ul. Wólczańska 215B
- Sports Centre — Al. Politechniki 10

### Use Cases

**UC-2.1 — Finding a building before the first day**  
A student wants to know where their faculty building is before classes start. They open the Map tab, browse the interactive campus map, and spot the building. They tap "Open full" to get directions from their location.

**UC-2.2 — Locating a facility on campus**  
A student needs to visit the Student Health Centre to register with a doctor. They open the Map tab, find the Health Centre in the quick-access list, note the address, and navigate there.

---

## 3. Timetable and Academic Organization (Schedules)

A centralized page linking students directly to their faculty's official timetable system.

### Features
- Faculty list with expandable dropdown cards
- Each card links to the faculty's official timetable page
- Clean interface with no extra clutter — just the faculty name and a direct link

### Faculties Covered
- IFE — International Faculty of Engineering
- BAIŚ — Civil Engineering, Architecture and Environmental Engineering
- WC — Faculty of Chemistry
- FTiMS — Technical Physics, Information Technology and Applied Mathematics
- WIPOŚ — Process and Environmental Engineering
- BiNoŻ — Biotechnology and Food Sciences
- WiW — Faculty of Textiles and Design
- WM — Faculty of Mechanical Engineering

### Use Cases

**UC-3.1 — Finding the class timetable**  
A first-year IFE student doesn't know where to find their schedule. They open the Schedules tab, tap the IFE card, and are taken directly to the IFE timetable page where they can select their year, programme, and group.

**UC-3.2 — Checking a schedule for a different faculty**  
A student wants to check when a friend from WM has classes. They tap the WM card and is directed to the Faculty of Mechanical Engineering's timetable page.

---

## 4. Centralized Student Platform (Profile)

A unified profile page and navigation system bringing all features together in one place.

### Features
- Bottom navigation bar with four tabs: Checklist, Map, Schedules, Profile
- Profile page showing name, email, faculty, and account status
- Editable profile fields: full name, email, faculty
- Password change with validation
- "My progress" section mirroring checklist completion
- Quick-access links to: WebDziekanat, WIKAMP, TUL email (SPE), Campus Map, Class Schedules

### Use Cases

**UC-4.1 — Setting up a profile on first use**  
After registering, a student opens the Profile tab and taps "Edit profile." They enter their full name and select their faculty from the dropdown. They save, and their name now appears across the app.

**UC-4.2 — Reviewing overall progress**  
A student opens their profile mid-semester to check how many onboarding steps they've completed. The "My progress" section shows each step with a done/to-do badge. They tap a pending step and are taken directly to the Checklist.

**UC-4.3 — Accessing university systems quickly**  
A student needs to check their grades. Instead of searching for the URL, they open the Profile tab and tap the WebDziekanat shortcut, which opens the portal directly.

---

## What Makes This Different

Most universities give new students a PDF, a generic student portal, and a list of links. This app takes a different approach — here's what sets it apart.

### Everything in One Place
First-year students at TUL currently have to juggle WebDziekanat, WIKAMP, faculty websites, mapa.p.lodz.pl, and their email just to get through the first week. This app consolidates all of it into a single, mobile-friendly interface. No more searching for the right link or remembering which system holds which information.

### Onboarding as a Guided Experience, Not a Document
Rather than handing students a checklist PDF they'll likely lose, the app turns onboarding into an interactive, persistent experience. Progress is saved to their account — so whether they complete two steps today and three next week, the app remembers exactly where they left off. This is something a static document or generic university portal simply cannot do.

### Personalisation Based on Faculty and Year
Unlike a one-size-fits-all student portal, this app is designed to adapt to the individual student. Once a student selects their faculty and year, the app surfaces the information most relevant to them — their faculty's timetable, relevant links, and tailored content — rather than presenting everything to everyone. A first-year IFE student sees IFE-specific resources by default; they don't have to dig through content meant for other faculties.

### Built for the Transition Period
Generic university portals are built for students who already know how things work. This app is specifically designed for the first few weeks — the most disorienting period of university life. Every feature (the checklist, the map, the schedules, the quick links) is chosen because it answers a question a new student is likely to have right now, not six months in.

### Campus Navigation Integrated with Academic Context
The map isn't just a standalone feature — it's connected to the academic experience. Students can use it in the context of finding where their classes are, not just as a generic map viewer. As personalisation develops, the map can surface directions to buildings relevant to the student's own timetable.

---

## Not Yet Implemented (from specification)

The following functionalities are described in the project specification but are not present in the current prototype:

- **Personalisation based on faculty** — different look for different faculty