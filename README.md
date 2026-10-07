<div align="center">

<img src="assets/android-chrome-512x512.png" alt="LOKAL logo" width="96" />

# LOKAL

### Your PowerPoint. A more interactive classroom.

[![README views](https://hits.sh/github.com/ke1thdev/LOKAL-Downloads.svg?label=README%20views&color=0d9488&labelColor=0b1f1c)](https://hits.sh/github.com/ke1thdev/LOKAL-Downloads/)

**Teach from PowerPoint. Let students participate from their browsers.**<br />
An offline-first classroom response, presentation, and engagement system.

[Download for Windows](https://github.com/ke1thdev/LOKAL-Downloads/releases) · [Getting started](#getting-started) · [Visual tour](#powerpoint-ribbon) · [Reports](#reports-and-rewards) · [Help and feedback](#help-and-feedback)

<img src="assets/open-graph.jpg" alt="LOKAL brings interactive activities to PowerPoint over a local classroom network" width="100%" />

</div>

---

## Meet LOKAL

LOKAL turns an ordinary PowerPoint lesson into a live classroom experience. Add a quiz to a slide, invite learners with a class code or QR code, collect their answers, review submissions, award stars, and keep a report of the session.

**Classroom use over a local Wi-Fi or wired LAN does not require an internet connection.** The teacher's computer runs the local LOKAL server; student devices need a reachable connection to that computer. An internet subscription is not needed for the local quiz itself.

LOKAL also includes presentation annotations, whiteboards, a name picker, quick polls, timers, individual and group leaderboards, a teacher dashboard, and Excel reports. Hosted access and cloud synchronization are optional, separately configured capabilities—not requirements for a local lesson.

This repository is for **public downloads and product documentation**. The Windows setup EXE is distributed through Releases. This is not the development codebase; classroom databases, credentials, student exports, private diagnostics, and development/test files should not be uploaded here.

### Explore this guide

- [Features at a glance](#features-at-a-glance)
- [Downloads and requirements](#downloads-and-requirements)
- [Getting started](#getting-started)
- [PowerPoint ribbon](#powerpoint-ribbon)
- [Classroom activities](#classroom-activities)
- [Activity options and live responses](#activity-options-and-live-responses)
- [Classroom tools](#classroom-tools)
- [Presentation toolbar](#presentation-toolbar)
- [Reset tools](#reset-tools)
- [Teacher dashboard](#teacher-dashboard)
- [Reports and rewards](#reports-and-rewards)
- [Student experience](#student-experience)
- [Server status and connectivity](#server-status-and-connectivity)
- [Help, About, and common questions](#help-and-feedback)
- [Privacy, authors, and license](#privacy-and-responsible-use)

> **About the visuals:** interface captures use fictional demonstration data. Native captures are rendered window/component previews without the surrounding Office desktop; some show selected option details rather than every control, and native window-region geometry may differ in a render. Ribbon/menu command guides are explicitly labeled illustrations, not screenshots. They explain the current commands without showing a real teacher account, classroom roster, or network address. Layout can vary with the installed version, screen size, and display scaling.

## Features at a glance

| Area | What you can do |
|---|---|
| Interactive slides | Add Multiple Choice, Word Cloud, Short Answer, Image Upload, and Fill in the Blanks activities. |
| Live participation | Invite learners by QR code, joining link, and class code; see submitted and pending participants. |
| Response review | Show or hide responses, search supported views, reveal configured answers, review images, and insert results as slides. |
| Rewards | Record automatic awards, manual rewards, and deductions; show class/session ranks and level badges. |
| Classroom utilities | Run a countdown or stopwatch, pick names, launch quick polls, and manage class groups. |
| Presentation tools | Annotate with pen, highlighter, shapes, and text; add whiteboards and move configured draggable objects. |
| Teacher dashboard | Manage classes, participants, groups, activities, reports, account information, and settings. |
| Reporting | Review session/activity details and download auto-scored, teacher-reviewed, complete, activity, and leaderboard Excel reports. |
| Local operation | Conduct classroom sessions over a reachable LAN without relying on a hosted server. |
| Optional connected features | Use configured online access and local-to-cloud synchronization when suitable infrastructure and internet connectivity are available. |

## Downloads and requirements

Download **LOKAL-Setup-x64.exe** from the [LOKAL release assets](https://github.com/ke1thdev/LOKAL-Downloads/releases).

| Component | Included in the Windows setup |
|---|---|
| LOKAL server | Receives classroom submissions, stores records, serves the browser pages, and delivers live updates. |
| PowerPoint add-in | Adds the LOKAL ribbon, slide activities, response windows, and presentation tools. |
| Server Status application | Provides joining information, service controls, connection assistance, release checks, and diagnostic access. |
| Installation prerequisites | .NET Framework 4.8 and the Visual Studio Tools for Office Runtime, installed when required. |

### What you need

- A **64-bit Windows computer** with a compatible desktop Microsoft PowerPoint installation.
- Administrator permission to install LOKAL.
- Student devices with a browser and a network connection that can reach the teacher's computer.
- A Wi-Fi access point/router or wired LAN that permits device-to-device communication for local classroom use.

PowerPoint is not included with LOKAL. PowerPoint for the web does not host the Windows desktop add-in. Learners do not need PowerPoint or the LOKAL add-in installed.

**Download the EXE listed under release assets.** GitHub's automatically generated “Source code” ZIP/TAR downloads are not the Windows installer. Read the release notes for version-specific changes and limitations.

Only obtain installers from the linked project releases. If Windows displays a publisher or reputation warning, verify the release/source before proceeding; do not disable Windows protection or install an unrelated certificate to suppress a warning. Use a published checksum when one is supplied.

## Getting started

### Install and prepare the teacher's computer

1. Save your presentation and close PowerPoint.
2. Download LOKAL-Setup-x64.exe, review the license, and install it with administrator permission.
3. Open **LOKAL Server Status** and check that the local server is running.
4. Reopen PowerPoint and select the **LOKAL** ribbon.
5. Choose **Sign In / Sign Up**. The teacher browser page handles authentication and can approve the PowerPoint sign-in.
6. Open **My Classes** to create a class, or use **Select Class** to choose an existing one.

After the setup file has been downloaded, installation can run offline using its bundled prerequisites. Optional Google sign-in or hosted features still require their configured online services.

### Run your first lesson

1. Select a class. LOKAL prepares a waiting room so learners can join before the activity begins.
2. Add one of the five quiz types to a slide.
3. Configure that slide in **Activity Options**.
4. Share the class joining link, QR code, and code.
5. Start the PowerPoint slide show.
6. Start the activity manually from its slide button, or enable **Start activity with slide**.
7. Review participation, close submissions when ready, and show the collected responses.
8. Award stars where appropriate and open **Reports** after the lesson.

Writing a question on a slide and inserting an activity are separate steps: design the prompt in PowerPoint, then configure how students answer it.

### How students join

1. Connect to the teacher's classroom network.
2. Open the joining address or scan the QR code.
3. Enter the active class code and participant name.
4. Optionally choose an avatar, then wait for the teacher's activity.
5. Submit the requested answer in the browser.

**Do not give students 127.0.0.1 or localhost as the joining address.** On a student's phone, those addresses point to the phone itself. Use the joining address displayed by LOKAL for the classroom network.

## PowerPoint ribbon

The **LOKAL** ribbon keeps lesson preparation, classroom tools, and browser-dashboard shortcuts together.

![LOKAL ribbon command guide showing the Me, Add quiz, and More groups](docs/screenshots/illustrations/ribbon-overview.png)

*Command-guide illustration of the current ribbon; not an Office screenshot.*

| Ribbon area | Commands and purpose |
|---|---|
| Me | Sign In / Sign Up; account access and Sign Out after authentication. |
| Add quiz | Multiple Choice, Word Cloud, Short Answer, Image Upload, Fill in the Blanks. |
| Class and dashboard access | Select Class, My Classes, Reports, Activities, Settings. |
| More features | Timer, Name Picker, Quick Poll, Leaderboard, Class groups, Draggable Objects, Share PDF. |
| Reset | Response reset and separate presentation cleanup commands. |
| Get help | Help and About. |

**Select Class** connects the presentation to its classroom. **My Classes**, **Reports**, **Activities**, **Settings**, and **My Account** open the appropriate teacher browser page; they are not additional native PowerPoint tabs.

<details>
<summary>View the More features and Get help command guides</summary>

![More features command guide](docs/screenshots/illustrations/more-features.png)

![Get help command guide](docs/screenshots/illustrations/help-menu.png)

*These are labeled command illustrations using LOKAL's current action names and assets.*

</details>

## Classroom activities

LOKAL provides **five slide-based activity types**, plus a separate Quick Poll utility for spontaneous questions during a slide show.

![The five current LOKAL Add quiz commands](docs/screenshots/illustrations/quiz-buttons.png)

*Illustrated Add quiz command guide; these are not captured on-slide activity buttons.*

| Activity | Learner response | Scoring/review |
|---|---|---|
| Multiple Choice | Select one answer or a configured set of answers. | Optional answer key and Quiz mode; answer-distribution chart and teacher review. |
| Word Cloud | Submit words or short phrases. | Frequency-based word cloud and teacher-awarded stars. |
| Short Answer | Write one or several permitted responses. | Read/search answer cards and award stars manually. |
| Image Upload | Upload an image or use an available camera; add a caption if configured. | Review images/captions, open previews, and award stars manually. |
| Fill in the Blanks | Enter an answer for each configured blank. | Optional accepted answers, capitalization rules, and Quiz mode; response table and manual bonus review. |

### Multiple Choice

Use it for knowledge checks, opinion questions, and questions with one or more correct choices.

- Configure **2–8 choices**, labeled A–H.
- Allow one choice or multiple selections.
- Optionally enable **Has correct answer(s)** and configure the answer key.
- Turn on **Quiz mode** to award automatic stars for correct submissions: Easy = 1, Intermediate = 2, Difficult = 3.
- Review the answer-distribution chart and open a choice to see its submitters.
- Use manual award/decrease controls in supported response-review views.

For a multiple-answer question, the selected answer set must match the configured correct set. Merely selecting one correct option is not enough. An answer key and Quiz mode are separate settings; **disabling the answer key turns Quiz mode off**.

<details>
<summary>View Multiple Choice options and response review</summary>

![Multiple Choice Activity Options](docs/screenshots/native/activity-options-multiple-choice.png)

![Multiple Choice response chart](docs/screenshots/native/responses-multiple-choice.png)

</details>

### Word Cloud

Use it to gather prior knowledge, keywords, ideas, reflections, and short phrases.

- Allow **1–5 entries per student**; student entries support up to 40 characters each.
- Optionally hide the cloud until you reveal responses.
- Repeated matching answers are grouped and become larger as their frequency increases.
- The cloud reflows as answers change, keeping the display readable.
- Toggle **Highlight top answer** to emphasize the most frequent entry or entries tied for the top frequency.
- Click a word to view its submitters and award/decrease stars.
- Right-click a word to remove it with confirmation; moderation is reflected in the recorded report.
- Insert collected results as a slide.

Word Cloud does not use an automatic answer key or automatic correctness rewards.

<details>
<summary>View Word Cloud options and response review</summary>

![Word Cloud Activity Options](docs/screenshots/native/activity-options-word-cloud.png)

![Word Cloud response window with demonstration submissions](docs/screenshots/native/responses-word-cloud.png)

</details>

### Short Answer

Use it for explanations, reflections, written reasoning, and open-ended questions.

- Configure one submission or allow **up to three**.
- Each written answer supports up to **1,000 characters**.
- Optionally hide participant names in presentation/review views.
- Search and read response cards.
- Add or decrease manually awarded stars using the available controls.
- Insert the collected answers into the presentation.

Hiding names changes what is shown to the audience. It does **not** delete the saved link between an answer and its participant.

<details>
<summary>View Short Answer options and response review</summary>

![Short Answer Activity Options](docs/screenshots/native/activity-options-short-answer.png)

![Short Answer response review](docs/screenshots/native/responses-short-answer.png)

</details>

### Image Upload

Use it for photographed work, visual examples, diagrams, and learner-created images.

- Accept student **JPEG, PNG, and WebP** images up to **5 MB**.
- Offer a file picker and a camera option when supported and permitted by the learner's browser/device.
- Configure an optional or required caption; student captions support up to 300 characters.
- Optionally hide participant names.
- Review thumbnails, search supported captions/names, and open larger previews.
- Award/decrease manual stars, download an image, or insert an individual image as a slide.
- Insert the collected results as slides.

A successful image submission is not replaceable through the same student answer view. Camera behavior and permission prompts depend on the device. A connection failure is not a successful upload—wait for the saved-submission confirmation.

<details>
<summary>View Image Upload options and response review</summary>

![Image Upload Activity Options](docs/screenshots/native/activity-options-image-upload.png)

![Image Upload response review using a fictional demonstration image](docs/screenshots/native/responses-image-upload.png)

</details>

### Fill in the Blanks

Use it for terms, calculations, short factual answers, and structured completion tasks.

- Configure **1–5 blanks**.
- Optionally provide accepted answers, with **up to five alternatives per blank**, separated by semicolons.
- Accepted answers and student entries support up to 30 characters per blank.
- Choose whether capitalization must match; surrounding spaces are ignored.
- Enable Quiz mode for 1, 2, or 3 automatic stars when the **overall response** is correct.
- Review a table with a student-name column and separate blank columns.
- Use the response table's **+1 star / −1 star** controls to adjust manually awarded stars repeatedly.

Manual adjustments apply to the student's **whole activity response**, not separately to each blank. Each confirmed +1 click adds one manual star; repeated clicks are supported. Manual deductions cannot reduce a response below its separately recorded automatic award, or below zero for an unscored response. Turning off the answer key also turns off Quiz mode.

<details>
<summary>View Fill in the Blanks options and response review</summary>

![Fill in the Blanks Activity Options](docs/screenshots/native/activity-options-fill-blanks.png)

![Fill in the Blanks response table](docs/screenshots/native/responses-fill-blanks.png)

</details>

## Activity options and live responses

### Configure each slide

Activity Options contains the activity-specific controls above and shared playback settings:

| Option | What it does |
|---|---|
| Start activity with slide | Starts collection when that configured slide is reached in the slide show. |
| Minimize activity window after starting | Keeps more of the slide visible while students answer; it does not end collection. |
| Auto-close submission | Uses the selected seconds/minutes deadline to close submissions. Leave it off to close manually. |
| Monitor tab switching | Records supported page-visibility signals and away/connection indicators for teacher review. |
| Save as default | Applies the current defaults to newly added activities of that type on this Windows account/computer. |
| View Responses | Opens available recorded/live responses; it does not create a new activity. |
| Activity Options Help | Opens the local guide at the relevant activity section. |

Changing a default does not rewrite activities already configured on other slides.

### Collect, reveal, and review

The response window brings together participation and review controls:

- A participant count and **Submission status** with submitted/pending participants.
- The activity clock and **Close submission** action.
- **Responses** show/hide control for the supported view.
- Additional time for timed activities.
- Correct-answer reveal after closure for configured Multiple Choice and Fill in the Blanks activities.
- Name visibility controls in supported anonymous-display views.
- Activity-specific charts, clouds, cards, tables, and image galleries.
- Star-award controls and **Insert as slide**.

**Minimizing or hiding a response window is not the same as closing submissions.** Reopen the activity's response view from its slide button or View Responses; do not start another attempt just to see the open activity.

<details>
<summary>View the activity countdown and local options guide</summary>

![Activity countdown indicator](docs/screenshots/native/activity-countdown.png)

![Built-in Activity Options Help](docs/screenshots/native/activity-help.png)

</details>

### Understand monitoring correctly

Page-switch indicators are **browser visibility signals, not proof of cheating**. Camera/file picking, interruptions, browser shutdown, refreshes, connection loss, and device behavior can affect the observations. “Connection lost—cause unknown” should not be interpreted as a confirmed tab switch.

### Keep attempts and counts meaningful

An empty start followed by closure is not a student submission. An attempt with no responses or response-award history is omitted from report/activity lists and counts; internal lifecycle records may still exist. Starting again creates a new attempt, and a saved zero-star answer still counts as a response.

Response totals count saved submissions, not merely the number of students multiplied by slides. Multiple Word Cloud words and Short Answer entries are not automatically separate student response rows.

## Classroom tools

### My Class and joining details

My Class is the presentation-side classroom workspace. Access it through the LOKAL presentation controls or the class-code badge.

- Share the class code, joining link, and QR code.
- Search participants, sort by join order/name, and show online participants.
- Adjust individual stars or award one star to everyone using **Award stars to all**.
- Lock the class against new joins.
- Open the leaderboard, name picker, quick poll, and class groups.
- Remove a participant with confirmation.

Starting a new class/session is different from refreshing the roster. It changes the session/joining context; confirm the intended class before proceeding.

<details>
<summary>View My Class</summary>

![My Class workspace](docs/screenshots/native/my-class.png)

*Fictional joining details and QR code are for illustration only, not a working classroom address.*

</details>

### Leaderboard

Celebrate participation with live ranking and level badges.

| Ranking mode | Measures |
|---|---|
| Current class rank | Stars earned in the current session. |
| Total stars rank | Accumulated stars in that class across sessions. |

The native leaderboard includes a podium, ranked participant rows, avatars, levels, live updates, and **Insert as slide**. Equal star totals share the displayed rank; response-time/name ordering can organize tied rows. While the teacher opens a live leaderboard, the selected view can also appear on connected student devices.

<details>
<summary>View the leaderboard</summary>

![LOKAL leaderboard with fictional participants](docs/screenshots/native/leaderboard.png)

</details>

### Timer and stopwatch

Use the standalone Timer for a classroom task even when no quiz is running.

- Switch between a countdown and stopwatch.
- Set minutes and seconds; start, pause, and reset.
- Adjust minutes while stopped.
- Choose and preview local alert sounds.

The general Timer is **separate from an activity's auto-close deadline**. Starting this utility does not automatically close a quiz.

<details>
<summary>View the Timer</summary>

![LOKAL Timer and stopwatch controls](docs/screenshots/native/timer.png)

</details>

### Name Picker

Choose learners without manually scanning the roster.

- **Card view** and **wheel view**.
- Online-only participant filtering and live roster refresh.
- Reveal/spin actions, randomization, and automatic picking of a chosen number of names.
- Picked-name history and **Put back**.
- Award a star to a selected participant.

The picker's Reset restores its selection pool/history—it does not reset classroom stars.

<details>
<summary>View card and wheel picking</summary>

![Name Picker card view](docs/screenshots/native/name-picker-cards.png)

![Name Picker wheel view](docs/screenshots/native/name-picker-wheel.png)

</details>

### Quick Poll

Ask a spontaneous question **during a live slide show** without preparing another activity button.

| Poll format | Choices |
|---|---|
| True / False | Two choices. |
| Yes / No / Unsure | Three choices. |
| Feedback | Five levels from Strongly disagree to Strongly agree. |
| Custom | 2–6 lettered choices. |

Quick Poll is single-choice and ungraded by default: it has no configured correct-answer key, Quiz mode, or automatic submission deadline. Review its live chart and use the supported manual-reward workflow.

Starting a new quick poll closes the currently active activity. Choose it intentionally rather than launching it over a question that is still collecting answers.

<details>
<summary>View Quick Poll</summary>

![Quick Poll format picker](docs/screenshots/native/quick-poll.png)

</details>

### Class groups

Support team-based engagement while keeping individual student records.

- Create groups and edit their names/colors.
- Search and manage members; retain an Ungrouped roster.
- Generate balanced random groups by group count or maximum students per group.
- View group ranks based on members' stars.
- **+1 each / −1 each** adjusts each current member, not a separate team-only score.

Random grouping replaces the existing group arrangement but preserves individual stars. Deleting a group returns its members to Ungrouped; it does not delete the students.

<details>
<summary>View the native class-group workspace</summary>

![Class groups using fictional participants](docs/screenshots/native/class-groups.png)

</details>

## Presentation toolbar

LOKAL's toolbar keeps presentation tools accessible at the bottom of the slide show.

![Current LOKAL presentation toolbar](docs/screenshots/native/presentation-toolbar.png)

*Rendered capture of the current native toolbar; the surrounding slide show is not included.*

| Tool | Classroom use |
|---|---|
| LOKAL / My Class | Open the live classroom workspace. |
| Slide Index | Navigate through slide thumbnails. |
| Previous / Next Slide | Move through the presentation. |
| Cursor / Laser Pointer | Point at content without leaving a permanent laser trail. |
| Pen / Highlighter / Eraser | Annotate, emphasize, or remove supported annotations. |
| Shapes | Draw rectangles, ellipses, triangles, lines, and arrows. |
| Text | Add annotations with configurable foreground/background colors. |
| Whiteboard | Insert a blank, patterned, or custom-background teaching slide. |
| Select Objects | Move/resize supported annotation objects. |
| Draggable Objects | Move slide objects that were configured as draggable. |
| Timer / Quick Poll / Name Picker / Leaderboard | Open the classroom utilities. |
| Hide / Show toolbar | Control toolbar visibility without ending the lesson. |
| Exit Slideshow | Return to editing. |

Pen/highlighter tools offer color and stroke-width choices. Saved LOKAL annotations become presentation content; temporary laser trails do not. Use the appropriate reset command when you want to remove saved annotations.

### Whiteboards, draggable objects, and PDF

- Choose bundled whiteboard backgrounds such as boards, grid/ruled/graph paper, and an X–Y axis, or use teacher-uploaded backgrounds.
- In editing view, select shapes/pictures/text boxes and mark them as **Draggable Objects**. The slideshow tool can move those configured objects.
- **Reset Draggable Objects** restores the recorded original positions.
- **Share PDF** exports a separate PDF copy using PowerPoint. It does not replace the active PowerPoint file.

<details>
<summary>View the whiteboard picker</summary>

![LOKAL whiteboard background picker](docs/screenshots/native/whiteboard.png)

</details>

Exiting the slide show allows presentation editing while keeping the classroom session. Closing PowerPoint ends the live presentation session. Keep the teacher computer and local server available while students are participating.

## Reset tools

Use the Reset menu carefully: these commands have **different scopes**, and deletion actions are not visibility toggles.

![Reset command guide](docs/screenshots/illustrations/reset-menu.png)

*Command-guide illustration; not a screenshot.*

| Command | Changes | Preserves |
|---|---|---|
| Delete All Responses | Removes the current session's responses and their credited automatic/manual **response-linked** stars. | Earlier sessions, separate session/group rewards, quiz slides, and already inserted result slides. |
| Reset Draggable Objects | Restores configured draggable objects to their original positions. | The objects themselves and unrelated slide content. |
| Reset Added Slides | Deletes LOKAL-added result, leaderboard, and whiteboard slides. | Original non-LOKAL slides. |
| Delete All Annotations | Removes saved LOKAL annotations. | Whiteboard slides and other presentation content. |
| Delete All Whiteboards | Removes LOKAL whiteboard slides. | Other slides and their annotations. |

Destructive deletion actions request confirmation. **Delete All Responses does not mean “reset every star a student has ever earned.”** The teacher dashboard has a separate class-wide **Reset stars** action. Back up important records before deletion or maintenance.

## Teacher dashboard

The browser dashboard complements PowerPoint with class administration, saved activity review, reports, and account/server settings. The screenshots below use demo fixtures, not a real class.

### Sign in and sign up

Sign in with a LOKAL username/password or create a teacher account through the guided registration flow. Registration collects username, password/confirmation, email, display name, organization, and profession.

Save the issued recovery code securely. The recovery workflow can restore access without depending on email delivery; use the saved code and follow the displayed connection/security requirements. Optional Google sign-in is shown only when configured.

<details>
<summary>View the browser sign-in and registration pages</summary>

![LOKAL teacher sign-in](docs/screenshots/web/teacher-login.png)

![LOKAL guided teacher registration](docs/screenshots/web/teacher-signup.png)

</details>

### My Classes / Classes

Create a class with a name, joining code, and a color/photo avatar. Class cards show participant/group counts. Sort classes by creation date, name, or participant count, and select individual/all cards for supported bulk operations.

Every class has five workspace tabs:

| Tab | Features |
|---|---|
| Participants | Add names, review name/group/stars/level, sort the roster, manage memberships, edit/remove participants, adjust stars, and download participant CSV. |
| Groups | Create/edit colored groups, manage members, generate random groups, show team totals/ranks, and award/decrease one star per member. |
| Reports | Open that class's saved sessions, browse Philippine month/year sections, favorite reports, and review their details. |
| Leaderboard | See accumulated class stars and download the class leaderboard as CSV. |
| Settings | Edit class name/code/avatar; reset participant stars or delete the class using explicit confirmations. |

Deleting a class can remove related records. Class-wide star reset is different from deleting a session's response-linked awards.

<details>
<summary>View Classes and all five class tabs</summary>

![Teacher Classes page](docs/screenshots/web/teacher-classes.png)

![Class Participants tab](docs/screenshots/web/class-participants.png)

![Class Groups tab](docs/screenshots/web/class-groups.png)

![Class Reports tab](docs/screenshots/web/class-reports.png)

![Class Leaderboard tab](docs/screenshots/web/class-leaderboard.png)

![Class Settings tab](docs/screenshots/web/class-settings.png)

</details>

### Reports

The Reports page brings together saved sessions across classes. Browse sessions by month, see awarded stars and top players, favorite a report, and open a Class Report.

A Class Report provides an activity timeline, recorded response counts, star totals, auto-scored question results, manual response review, and session rankings. Open an activity for its own detailed report.

<details>
<summary>View the report list, Class Report, and activity report</summary>

![Teacher Reports page](docs/screenshots/web/teacher-reports.png)

![Detailed Class Report](docs/screenshots/web/session-report.png)

![Individual activity report](docs/screenshots/web/activity-report.png)

</details>

### Activities

Browse **recorded past activities**, filter by quiz type, sort by date/favorites/response count, and open an activity's report from its slide thumbnail.

This is a review library—not a browser-based slide or quiz builder. Prepare slide activities in PowerPoint.

<details>
<summary>View Activities</summary>

![Teacher Activities library](docs/screenshots/web/teacher-activities.png)

</details>

### Settings

| Functional area | Features |
|---|---|
| Connection | View/select the operating mode and joining/dashboard addresses; manage configured online/sync connection details. Listener changes may require a server restart. |
| Star Levels | Edit star requirements, add/remove supported levels, and use supplied badge artwork. |
| Whiteboard Backgrounds | Upload, preview, and remove supported custom backgrounds for the PowerPoint whiteboard picker. |

The Notifications area is currently an **available-soon placeholder**, not an implemented notification-preference system.

<details>
<summary>View Connection, Star Levels, and Whiteboard Backgrounds</summary>

![Connection settings](docs/screenshots/web/settings-connection.png)

![Star Levels settings](docs/screenshots/web/settings-star-levels.png)

![Whiteboard Backgrounds settings](docs/screenshots/web/settings-whiteboards.png)

</details>

### Account

Review/edit your teacher profile, manage a supported account photo, and view registered browsers/PowerPoint installations. Supported security workflows include recovery-code replacement and signing out other active devices.

Keep recovery codes private; LOKAL does not display them in this public guide. Optional Google account linking/unlinking depends on the configured provider.

<details>
<summary>View Account</summary>

![Teacher Account page using fictional profile data](docs/screenshots/web/teacher-account.png)

</details>

## Reports and rewards

### Stars and correctness are different

**Stars are classroom rewards—not automatically academic grades.** Correctness checking describes the submitted answer. Manual rewards can increase a learner's stars independently of whether that answer was correct.

Report categories follow the scoring mode recorded for the **activity attempt**:

| Item | Where it belongs |
|---|---|
| Automatic stars for a scored Multiple Choice/Fill in the Blanks run | Automatic-star component of auto-scored activity totals. |
| Teacher bonus on that same auto-scored run | Manual-bonus component of the **auto-scored** category. |
| Manual stars on a Word Cloud/Short Answer/Image Upload run | Teacher-reviewed activity totals. |
| Multiple Choice/Fill in the Blanks run without Quiz mode | Teacher-reviewed category. |
| Separate participant/session/group reward | Outside-quiz awards included in the overall session total where associated with that session. |
| Historical balance without reliable award-source evidence | Clearly marked as unclassified; not guessed to be automatic or manual. |

Deductions affect net reward totals. **Within response review**, manual deductions cannot reduce a response below its separately recorded automatic award. This protection does not mean that automatic awards survive response deletion or a deliberate class-wide reset.

**Total session stars** includes the session's categories and associated outside-quiz awards. **Class leaderboard stars** accumulate across sessions. These are different scopes; do not add category totals to the total again or repeatedly sum a participant's session total on each response row.

### What the report shows

- Session overview: class code, recorded activities, submitted responses, stars awarded, and top players.
- Activity timeline: slide preview, question/activity label, type, timing, response/star totals, and scoring category.
- Auto-scored questions: submitted answers, correctness, difficulty, correct percentage, average response time, automatic/manual/unclassified components, category total, and total session stars.
- Manual response review: question/type, full answer or preview, response stars, reviewed-category components/totals, total session stars, response time, and submission time.
- Individual activity reports: response distributions, word frequencies, text answers, blank columns, or image galleries, plus relevant student-level details.
- Excel star-history sheets: award source and committed changes, including deductions where applicable.

Manual review supports opening words, full text, and images. Names hidden in a presentation/review are still associated with stored records, and exports include participant names.

### Excel and CSV downloads

| Download | Scope and contents |
|---|---|
| Auto-scored report | Only scored activity runs, with their automatic awards **and manual bonuses**; Summary, Responses, and Star history sheets. |
| Teacher-reviewed report | Activity runs with Quiz mode off and their manual awards; its own Summary, Responses, and Star history sheets. An answer key may still check correctness without automatic rewards. |
| Complete report | Both categories, complete-session totals, activity details, student results, response records, and award history; additional outside-quiz award details when present. |
| Activity report | The selected activity and its response/reward details. |
| Session leaderboard | Session ranking export, with Excel and CSV options. |
| Class leaderboard / participants | Supported class-level CSV exports. |

The complete workbook starts with **Complete summary** and includes the auto-scored and teacher-reviewed sections rather than presenting only automatic quizzes as the whole session.

Workbooks use LOKAL author/last-modifier branding, readable column widths, wrapped headers/answers, styled rows, frozen panes, filters, and useful numeric formats. Very long answers remain in cells and may require expanding the row in Excel.

### Time and saved data

Teacher report displays and human-readable exported dates use **Philippine Standard Time: Asia/Manila, UTC+08:00**. Technical database/API/log timestamps and workbook internal creation metadata may remain UTC; those are not the displayed classroom time.

Report pages refresh from saved data while visible. A temporary connection failure can leave the last confirmed view on screen. Wait for submission/award confirmation and refresh or reconnect if an action reports an error; the system cannot guarantee that an unacknowledged network request was saved.

## Student experience

Students use the teacher's joining page in a browser—no add-in installation or student password is required for the classroom join workflow.

- Join using the current code/name and an optional avatar.
- View the active activity and answer from a phone, tablet, or computer.
- See the submission receipt and supported response-time feedback.
- Follow synchronized activity deadlines and receive warning/expiry sounds.
- Receive recorded star updates, reward animations, level badges, and level-up feedback.
- See teacher-shared live session/class leaderboards.
- Use the student light/dark theme and supported fullscreen view.
- Rejoin/reload on the same browser/device to restore supported participant/submission state.

Changing an answer is available for supported open activities unless an award locks that response. Short Answer has its own additional-entry/removal rules; Image Upload does not offer post-submission image replacement.

<details>
<summary>View the student joining and activity screens</summary>

![Student class-code joining page](docs/screenshots/web/student-join.png)

![Student activity answering view](docs/screenshots/web/student-activity.png)

</details>

## Server status and connectivity

The Windows Server Status app is the teacher's local service companion. Use it to view joining details, check the server, start/stop/restart it where permitted, investigate a connection issue, verify installed release files, and access diagnostics.

<details>
<summary>View the Server Status application</summary>

![LOKAL Server Status in an isolated disconnected demonstration](docs/screenshots/native/server-status.png)

*Rendered disconnected Offline-mode demo, not a reading of the installed service. Its localhost address is for the teacher computer only, not for students on other devices.*

</details>

| Mode | Typical use | Internet needed? |
|---|---|---|
| Computer-only / Offline mode | Work on the teacher computer without permitting student LAN access. | No. |
| Local Network mode | Students connect to the reachable teacher server over the same classroom LAN/Wi-Fi. | No for the local session. |
| Configured Online access | Use an appropriately configured hosted/proxy/tunnel address. | Yes. |
| Optional cloud synchronization | Send queued local changes to an enrolled hosted server. | Yes when synchronizing. |

**Offline-first classroom use means Local Network mode without internet—not that devices can communicate with no network at all.** LOKAL does not create a Wi-Fi hotspot. Guest Wi-Fi/client isolation, firewall restrictions, changing LAN addresses, or weak signal can prevent joining or submissions.

Cloud synchronization is opt-in **local-to-cloud** operation. Do not assume automatic bidirectional conflict resolution or that a hosted service is always available. Hosted access, Google sign-in, and synchronization depend on their configured infrastructure.

Local plain-HTTP classroom traffic is not encrypted end to end. Use trusted networks and appropriately configured HTTPS for hosted access. Do not expose the local port directly to the public internet or publicly share account tokens.

## Help and feedback

### Built-in Help and About

**Get help → Help** opens the local activity-options guide. It provides activity-specific instructions and shared playback/review guidance. The browser Help Center adds setup, network, reporting, update, and troubleshooting topics, with search and printing support.

**Get help → About** shows product information, authorship, and installed component/server versions.

<details>
<summary>View Help Center and About</summary>

![LOKAL Help Center](docs/screenshots/web/help-center.png)

![LOKAL About window](docs/screenshots/native/about.png)

</details>

### Common questions

<details>
<summary>Does LOKAL need the internet?</summary>

Not for a local classroom lesson. The teacher server and student devices need a reachable local network. Internet is needed to obtain the installer initially and for configured hosted/Google/cloud capabilities.

</details>

<details>
<summary>Do students need to install anything?</summary>

No LOKAL student app or PowerPoint add-in is needed. Students join and answer in their browser. Browser compatibility, camera permissions, and device resources still affect available behavior.

</details>

<details>
<summary>Can I prepare activities outside a slide show?</summary>

Yes—add and configure activity buttons while editing the deck. Live activity launch and Quick Poll are designed for PowerPoint slide-show use. Do not assume every alternate PowerPoint viewing mode has the same support.

</details>

<details>
<summary>Does closing/minimizing a response window stop the quiz?</summary>

No. Use Close submission or the configured auto-close deadline to end collection. Reopen the activity view to review its controls and responses.

</details>

<details>
<summary>Why are session stars different from the class leaderboard?</summary>

The session view covers rewards associated with that lesson. The class leaderboard covers accumulated stars across sessions. Manual bonuses and outside-quiz rewards can also make stars differ from pure correctness scores.

</details>

<details>
<summary>Does an empty activity count as a recorded quiz?</summary>

An attempt with no responses or response-award history is omitted from report/activity lists and counts. Saved responses with zero stars still count. Starting an activity is not itself a student answer.

</details>

<details>
<summary>How many students can participate?</summary>

Capacity depends on the teacher computer, network quality, activity type, image sizes, and submission timing. Read the release's load-test notes and test your intended class on the actual classroom network. Simulated load-test results are not a guarantee for every phone, Wi-Fi environment, or laptop.

</details>

<details>
<summary>Are names hidden permanently when anonymous display is enabled?</summary>

No. It masks the supported presentation/review view; identity linkage remains in saved records and named exports. Written responses, captions, and images can also identify their authors.

</details>

### Report a problem

For non-sensitive bugs, [open a LOKAL issue](https://github.com/ke1thdev/LOKAL-Downloads/issues) with:

- LOKAL release version and Windows/PowerPoint/browser versions as applicable.
- The activity type and steps that reproduce the issue.
- Expected behavior and what actually happened.
- A fictional/anonymized example or screenshot.

Do not upload real student reports, databases, private diagnostics, recovery codes, tokens, passwords, or private keys. Use an established private channel for sensitive security reports; do not publish exploit details or credentials in a public issue.

## Privacy and responsible use

LOKAL can store participant identities, avatars, answers, uploaded images, response timing/visibility observations, and reward history. Use it only on authorized computers/networks and follow your institution's data-handling rules.

- Use fictional records for demonstrations and public screenshots.
- Obtain appropriate consent and avoid unnecessary personal information.
- Back up important classroom data before updates, resets, or maintenance.
- Restrict access to the teacher computer and reports.
- Consider device encryption for protection if a computer is lost or stolen.
- Treat exported named reports as private classroom records.
- Remember that favorites and retention settings can affect how long report media is retained.

LOKAL is an academic project. Review the release notes and evaluate it in your environment before consequential assessments. No README claim replaces a classroom pilot, a backup, or an independent security review.

## Project authors

Developed as an academic thesis project by **Keith Renz D. Romblon** and **Camille R. Ramilo**.

LOKAL is independent and is not affiliated with or endorsed by Microsoft or ClassPoint. Product names belong to their respective owners.

## License

Use and distribution are governed by the [LOKAL software license agreement](installer/bootstrapper/EULA.txt), also presented by the Windows installer. A public download on GitHub does not itself grant an open-source license.

---

<div align="center">

**LOKAL · Interactive classrooms, directly in PowerPoint.**

[Get LOKAL](https://github.com/ke1thdev/LOKAL-Downloads/releases) · [Report a non-sensitive issue](https://github.com/ke1thdev/LOKAL-Downloads/issues)

</div>
