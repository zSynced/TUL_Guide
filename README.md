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

## Feedback
- Cite is build very clearly and easy to use. Even without additional information I could easily navigate it. I think it would be a lot easier for new students to navigate their studying and save them a lot of nerves :)
  
- The campus map is pretty good, suitable for beginners and even those who constantly forget everything, but it does lag a bit sometimes. The checklist is a good idea, but making it separate tab just waste of screen , leaving it in the profile tab would be enough. The fact that you can view your schedule is also really cool.
  
- So it's pretty good so far, the nitpicks i have are mostly design stuff, like adding some sort of color pallete for it not to just be grey or smth. The design is intuitive and I like it! Don't really have a lot of problems with it other than that, though adding a FAQ would probably be appreciated

- The website is extremely helpful. 
Checklist is present on the front page PLUS in profile, which is like a double check.
Several useful links in maps help to prevent the confusion in buildings. Perfect to see before arriving and after, to walk around and not get lost.
“Schedule” page provides links straight to the needed time tables  for various of courses, which reduces time taken to find them and again avoids the confusion that could have been caused in alone search.
Useful links help to check the information if needed, as well as give an opportunity to read what the university has to offer more comprehensively. 
Also! Gives straight way to contact student support in case if needed. In my opinion this is one of the most useful tools an applicant can ask for.

- Overall, I like the vibe and usability of the website. The navigation is easy to follow, and I can access all the important information within one click. However, the layout currently feels strictly mobile-first, on a laptop screen it looks a bit constrained, like I'm looking at a phone screen embedded on a monitor (everything forced within a centered box) . While it works perfectly on my phone, I probably wouldn't use the desktop version as it currently stands. Also, it might be worth making the layout more responsive to utilize the wider desktop screens. (Tbh it looks a bit template-heavy or AI-sh, but the core concept is good) Things you might want to look into: text size on the mobile is perfect but some parts read too small on a laptop, adding an accessibility toggle might help. Also, you might consider adding a switch between themes like light and dark, the current usage of white background and black text/lines look very much like a word doc. I loved the idea of the embedded map, but it needs a bit tweaking to be more practical. The current map box is quite uncomfortable for both phone and laptop screens. If the goal is just to showcase the map and have students use it on the actual website, you might consider making the entire map preview clickable, so it automatically redirects user to nav.pl. Alternatively try to scale the embedded box to fit into different screen measurements. Also, you might consider adding more key locations and grouping in futher versions of the website, ex., a category for Administrative Buidings (Listing all dean's offices) or Dorms (listing all the available housing) etc. Also, I'm not quite sure what was the exact goal of checklist, but you might want to refine its operation. If the onboarding process is supposed to be sequential, you shouldn't allow users to check boxes in a chaotic random order, consider locking future steps until previous ones are completed. It might also be a good idea to disable the ability to uncheck the box to prevent accidental progress loss.  One more thing, I am not entirely sure how the ELS process works for international students (I remember trying to do it and failing to add the id) so it's definitely worth double-checking and mentioning if such students are able to accomplish that or not.  And some of the links towards timetables open wikamp login window instead, like for weeia, idk where they have their timetables so maybe it's normal.
And, I would have also considered having a page with links to some clubs or student activity they might want to join as it needs some digging to find out how or where to apply to some less known things. (Oh and our uni has Instagram and tiktok and some other social media you might consider adding that)
Other than that the idea is quite good, as a person who likes creating checklists for my todo lists I would have used the website during my enrolment process to keep the progress of it in check as well as make sure I know what my next steps are.

- The website is very useful because all the important information is one click away. What is more, you can access the website with both a computer and a phone. 
The progress of registration, which is tracked, makes it much easier for a student to see what is already done and what is still missing. An accessible timetable for all the departments at the same place makes the website even more usable for all the students. Also, the map of the campus, which already has important spots (such as the rector's office or student self care) marked seems to be a great idea. I would also add dorms or IFE of building to the map, because these are places all students will need in the first place.
So, from the practical point of view, the website is made really well (except the remark made about the map). For the future, it will be a good idea to slightly improve the design, for example, by adding the university colors.

- What I liked:
Simple design: In my opinion, it fits this type of website perfectly.
Content: The core content is quite useful — the checklist, the map, and the faculty info are all good.
What needs to be fixed/improved:
Profile page: I didn’t quite get why a profile is even needed on this site, but since it's there, it needs to stand out more. Personally, when I first looked at the site, I didn't even realize right away that I had landed on the profile page.
Navigation (Mobile UX): The navigation menu should be moved from the bottom to the top. It’s annoying to have to scroll down every single time just to switch sections (even though the pages are short). Plus, when you switch pages, it awkwardly loads from the bottom first. If moving it to the top isn't an option, you should at least make it a sticky/fixed menu so it stays in place, like a standard mobile layout.
State persistence: This might be obvious, but I'll mention it anyway: actions aren't saved when you refresh the page. Everything resets to default.
Map functionality: When I click on "key locations," the map doesn't show them. Not sure if it's supposed to be like that or if it's a bug.
Visual style (Emojis): I get that this is just a draft, but the emojis don't really fit the vibe. Also, considering they look different on almost every device, it's better to replace them with universal icons.

- Cool website—I like that it loads quickly. However: the interactive map loads slowly, checkpoint elements aren’t saved, the design is a bit boring, and there aren’t many helpful links at the checkpoints. I understand you’re embedding the interactive map via an iframe on some website; consider using a JavaScript library for maps (like leaflet.js) that will also let you make the map zoom in on specific locations when clicked.
Also, increase the margin/padding on the sides; on phones with curved screens, it’s essentially non-existent.
Or just remove the padding on mobile devices using a CSS media query with the appropriate query (as far as I recall, you can use max-width with the appropriate width).

- it is also good in the map if we mark the IFE building as an important one because is the Erasmus officine. Also in the first part (checklist) it can be good if we include another mark for OLA (Online Learning Agreement), which is a document that Erasmus people need to upload
  
---

## Not Yet Implemented:

- **Personalisation based on faculty** — different look for different faculty
- Correct gramatical issues/inconsistencies
- make the timetables show up based on picked faculty in profile section
