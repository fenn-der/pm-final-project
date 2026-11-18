# Competitive Analysis & Journey Map (Module 2)

## Responses
- **Role, who are you solving for? (the specific user segment or profile):** A dispatcher at a regional delivery fleet who coordinates drivers’ routes in real time across a shift.
- **Goal, what is this user ultimately trying to achieve?:** To redirect drivers the moment plans change and trust that the dashboard shows the true status of every stop.
- **Friction, the main barrier (moment of misery) stopping them from succeeding:** They reassign a route, and the driver doesn’t see the change for 10–15 minutes because there’s no push notification. By then the driver has already driven the wrong way (UXR-02, BUG-2044). On the night shift, the dashboard shows stops as “in progress” up to an hour after they were delivered (UXR-09, BUG-2072). The board can’t be trusted, so one fleet now runs its real coordination through a WhatsApp group.
- **External tools, the outside platforms or tools the user is forced to use:** A WhatsApp group used as “the real system” for route changes (UXR-02), text messages from drivers confirming deliveries instead of using the app (UXR-01), and phone calls to the office when the app crashes and loses a driver’s route (UXR-03).
- **The process, the 3 to 5 manual steps the user takes to get the job done:**
1. Reassign the route in RouteLogic.
2. Post the same change in the WhatsApp group so the driver sees it immediately instead of 10–15 minutes later.
3. Receive delivery confirmations from drivers by text rather than through the app.
4. Reconcile the chat against the dashboard, treating WhatsApp as the truth where they disagree.
5. Handle app crashes by phone, reading remaining stops to the driver.
- **Core frustration, the exact moment the process feels most “broken”:** The moment a dispatcher reassigns a route and realizes the driver won’t see it for 10–15 minutes, by which point the driver has already driven the wrong way. The tool built for real-time coordination can’t deliver a change in real time.
- **The evidence, a specific quote or behavior from the research that proves this:** “I reassign a route and the driver doesn’t see it for ten, fifteen minutes. By then they’ve driven the wrong way. We keep a WhatsApp group as the real system.” (Fleet dispatcher, mid-size 3PL, UXR-02). This is confirmed by BUG-2044: reassignments take 8–15 minutes to reach drivers, with no push notification.
- **Your journey map, a shareable link, or the map file you committed (e.g. journey-map.html):** https://github.com/fenn-der/pm-final-project/blob/89ffeff993c3944db7f99fd9a50d9cb8a761de3b/02-discovery/journey-map.md
