Naija Hustle + Lagos Life systems merge
This package was reconstructed from the saved Naija Hustle Surpass bundle in the project library (saved 8 October 2026). It is a recovery/merge build, not a guarantee that it contains every edit made after that saved snapshot.
Files
index.html — game interface, including LAPO/NEPO start buttons and the Focus meter.
styles.css — interface styling.
app.js — Three.js world, movement, avatar customizer, jobs, gigs, housing/rent, needs, inventory, shops, transport, investments, NPCs, relationships, quests, and local saves.
favicon.svg, logo.svg — existing game graphics.
Merged from Lagos Life
LAPO start: ₦12,000, basic room, phone, Hustler trait.
NEPO start: ₦150,000, self-contained home, phone/laptop, Owambe Spirit trait.
Traits: Hustler, Foodie, Owambe Spirit, Clean Pikin, Lazy Bone (the two starts grant Hustler or Owambe Spirit; the other traits are defined for further expansion).
Focus need added to state and HUD.
Added Elegushi Beach and Church / Mosque to the 3D destination list.
Added location actions for eating out, socialising, fun, grooming, workouts, and quick gigs.
Existing Naija Hustle jobs, skills, shops, six housing tiers, quests, businesses, and transport were preserved.
Repairs included
Fixed the renderInventory() missing parenthesis.
Removed duplicate updatePrompt() declaration.
Prevented the world from auto-starting before login/guest selection and added a start-once guard.
Restored saved player position after loading.
Added missing Focus need support for existing saved games.
Prevented repeated vehicle purchase charges for vehicles already owned.
Disabled unavailable/current housing move buttons.
Important limitations
The bundle passed Node's ES-module syntax check and a static HTML-ID lookup check. It has not been fully browser-tested on desktop/mobile after deployment.
Supabase sign-in still depends on the configured Supabase project and network access. Full progression is still local-first; this merge does not implement server-side cloud saving of all game progression.
Rent remains on the existing Naija Hustle 14-day cycle to avoid silently changing the existing economy. The new Lagos Life start types and activities are integrated with that economy.
Do not overwrite a live deployment until you test this recovery build first.
