![preview](https://raw.githubusercontent.com/narenkarthikeyanu999/charmed-recess/main/shot_c42f59.svg)
# 🎓 Spellbound Schoolyard: Chalkline Chronicles

[![Download](https://raw.githubusercontent.com/narenkarthikeyanu999/charmed-recess/main/btn_9e5e1.svg)](https://narenkarthikeyanu999.github.io/charmed-recess/)

![Luau](https://img.shields.io/badge/Luau-4.6-00A2FF?style=for-the-badge&logo=lua&logoColor=white)
![Declarative](https://img.shields.io/badge/World-Manifest-FF6B6B?style=for-the-badge&logo=json&logoColor=white)
![Cooperative](https://img.shields.io/badge/Co--op-Charm%20Loop-8A2BE2?style=for-the-badge&logo=handshake&logoColor=white)
![Portable](https://img.shields.io/badge/Runs%20Across-Devices-2ECC71?style=for-the-badge&logo=rocket&logoColor=white)
![MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge&logo=opensourceinitiative&logoColor=black)
![Year](https://img.shields.io/badge/Release-2026-blueviolet?style=for-the-badge&logo=calendar&logoColor=white)

---

## 🧭 A Different Kind of Playground

Spellbound Schoolyard: Chalkline Chronicles is an open, portable charm-collecting adventure where a scrappy crew of schoolyard kids trade playground rhymes for real magic. Instead of shipping a monolithic binary, this project treats the entire game world as a **declarative manifest** — a single, human-readable document that describes every chalk circle, hopscotch rune, and whispering swing set. The rules that bring that world to life are written in Luau, a nimble scripting language that keeps the logic close to the player and far from the boilerplate.

This repository is a reimagining of the original Spellbound Schoolyard concept, but it refuses to be a sequel or a reskin. Where the first game invited you to collect charms, Chalkline Chronicles invites you to **draw** them. Every charm is sketched onto the pavement by the collective effort of up to four players, and the schoolyard itself remembers what was drawn — even after the bell rings. The world manifest is the memory; the Luau rules are the heartbeat.

The result is a game that feels less like software and more like a recess ritual. It boots fast, runs light, and treats cross-device portability as a first-class citizen rather than an afterthought. Whether you are on a tablet, a handheld, or a desktop, the chalk lines appear at the same thickness, the same rhythm, the same warmth.

---

## 🌟 Why Chalkline Chronicles Exists

Most cooperative games ask you to shout over each other in a frantic race. Chalkline Chronicles asks you to **listen**. The core loop is built around a shared drawing surface where each player contributes a stroke, a rune, or a rhyme. The manifest defines what those contributions mean; the Luau rules decide how they combine. A charm is never owned by one player — it is owned by the circle of friends who conjured it.

This design choice ripples outward. It means the game has no single-player fallback that feels like a compromise. It means the difficulty curve is negotiated, not dictated. And it means the schoolyard is a character in its own right, one that evolves as the manifest is extended by the community.

The project is deliberately small enough to read in an afternoon but deep enough to reward a season of tinkering. It is a portable example, yes, but it is also a **teaching artifact** — a way to show newcomers how a declarative world manifest and a lightweight rule engine can conspire to make something that feels alive.

---

## ✨ Feature Highlights

- 🎨 **Manifest-Driven World** — Every chalk circle, swing set, and hopscotch rune is described in a declarative manifest, so the world can be reshaped without touching a line of game logic.
- 🧩 **Luau Rule Engine** — Charm behavior, cooperation thresholds, and rhyme combinations are expressed in Luau, keeping gameplay rules transparent and moddable.
- 🤝 **Cooperative Charm Loop** — Up to four players draw, rhyme, and collect charms together; no player can hoard a charm that was conjured by the group.
- 📱 **Responsive UI** — The interface adapts to handheld, tablet, and desktop screens without losing the hand-drawn aesthetic or the clarity of the chalk metaphor.
- 🌍 **Multilingual Support** — Rhymes, prompts, and charm names are localized, with a structure that welcomes community translations for new dialects and playgroups.
- 🕰️ **24/7 Customer Support** — A rotating team of maintainers and community stewards keeps the issue tracker warm and the documentation current, around the clock and around the calendar.
- 🔄 **Portable Core** — The same manifest and Luau rules run across supported devices, so progress and charm collections travel with the player.
- 🧠 **Readable Architecture** — The separation between world data and rule logic is enforced by convention and tooling, making the codebase approachable for first-time contributors.
- 🌱 **Community-Extensible** — New charms, schoolyard zones, and seasonal events can be added through pull requests that touch only the manifest and a small Luau module.
- 🧾 **Self-Documenting Manifests** — The manifest schema is annotated inline, so the world file doubles as a guide for anyone who wants to build their own schoolyard.

---

## 🗺️ How the Schoolyard Is Organized

The repository is structured around a simple metaphor: the **playground**, the **chalk**, and the **bell**.

- **The Playground** holds the manifest — the declarative description of every zone, prop, and charm anchor. It is the map, the memory, and the mood.
- **The Chalk** holds the Luau rules — the scripts that interpret the manifest, resolve cooperative actions, and decide when a charm is born.
- **The Bell** holds the orchestration — the boot sequence, the device abstraction layer, and the localization pipeline that rings changes across languages and screens.

This three-part split is intentional. It keeps the world data separate from the logic that animates it, and it keeps both separate from the plumbing that delivers them. A contributor who wants to add a new charm never needs to touch the boot sequence. A translator who wants to add a new dialect never needs to read a single line of Luau. A maintainer who wants to improve performance never needs to understand the rhyme schema.

---

## 🧒 The Cooperative Charm Loop, Explained

The charm loop is the beating heart of Chalkline Chronicles. It unfolds in four gentle movements:

1. **Gather** — Players assemble in a schoolyard zone. The manifest defines which charms are available in that zone and what conditions must be met.
2. **Draw** — Each player contributes a chalk stroke. The strokes are combined according to Luau rules that weigh order, proximity, and rhyme.
3. **Rhyme** — Players speak or select a rhyme that matches the drawn shape. The rhyme is the key; the drawing is the lock.
4. **Collect** — If the rhyme and drawing align, a charm is conjured and added to the shared collection. No single player owns it; the circle owns it.

The loop is deliberately slow enough to encourage conversation and fast enough to feel like play. It rewards patience, listening, and the kind of unspoken coordination that happens when friends share a piece of pavement.

---

## 🧰 Technology Choices and Their Consequences

**Luau** was chosen because it is small, fast, and friendly to newcomers. It runs close to the metal without demanding that contributors learn a sprawling toolchain. It also has a syntax that reads like prose, which matters when the rules are meant to be read by players as much as by programmers.

**A declarative manifest** was chosen because it makes the world inspectable. You can open the manifest in a text editor and see the whole schoolyard laid out before you. You can diff it, review it, and merge it without fear. The manifest is not a config file hiding in a corner; it is the centerpiece.

**Portability** was chosen because play should not be gated by hardware. The core is written to run across supported devices, with a thin abstraction layer that handles input, display, and storage differences. The goal is not to be everywhere, but to be where the players already are.

**Localization** was chosen because rhymes are cultural. A charm that works in one language may need a different rhythm in another. The localization pipeline is built into the boot sequence from the start, not bolted on at the end.

---

## 🧪 Testing and Verification Philosophy

The project treats tests as **chalk outlines** — faint guides that keep the drawing honest. There are three layers:

- **Manifest Validation** — The manifest is checked against a schema so that malformed zones, orphaned charm anchors, and missing references are caught before runtime.
- **Rule Simulation** — Luau rules are exercised in a headless harness that simulates cooperative players, verifying that charm conjuring behaves consistently across edge cases.
- **Device Smoke Runs** — A small suite of smoke runs confirms that the boot sequence, localization pipeline, and device abstraction layer behave as expected on each supported target.

The philosophy is simple: tests should be readable, fast, and close to the domain. A test that describes a charm-conjuring scenario should look like a charm-conjuring scenario, not like a stack trace.

---

## 🌐 SEO-Friendly Integration, Naturally

This repository is built to be discovered by the people who need it: educators looking for cooperative play examples, hobbyist developers curious about declarative world design, and translators who want to bring a small game into their own language. The documentation uses natural language that describes what the project **is** and what it **does**, rather than stuffing keywords into corners. Phrases like "portable cooperative charm-collecting game," "declarative world manifest," and "Luau rule engine" appear where they belong, in sentences that explain them.

The goal is not to trick a search engine but to **welcome a reader**. Every section is written to be useful to a human first, and discoverable to a machine second.

---

## 📱 Responsive UI and Multilingual Support in Practice

The responsive UI is not a single layout that stretches. It is a family of layouts that share a common vocabulary. On a handheld screen, the chalk strokes are thicker and the rhymes are shorter. On a tablet, the schoolyard breathes with more negative space. On a desktop, the manifest editor and the live preview sit side by side.

Multilingual support is not a translation dump. It is a **rhyme-aware pipeline** that treats each language as a distinct playgroup with its own rhythm, idioms, and charm names. The manifest schema includes optional rhyme overrides per locale, and the Luau rules read those overrides when resolving charm conjuring. Adding a new language means adding a folder, not rewriting a game.

---

## 🕰️ Around-the-Clock Stewardship

The 24/7 customer support model for this project is community-driven and rotation-based. Maintainers from different time zones share the responsibility of triaging issues, reviewing pull requests, and answering questions. The goal is not to have a hotline but to have a **warm presence** — someone who can help a newcomer unblock themselves at three in the morning, in their own time zone, without waiting for a business day.

This model is documented in the contributor guide, along with expectations for response times, escalation paths, and the handoff ritual between rotations. It is a small thing, but it is the difference between a project that feels abandoned and one that feels alive.

---

## 🧾 Manifest Schema at a Glance

The manifest is organized into top-level sections that mirror the schoolyard metaphor:

- **Zones** — Named areas such as the Hopscotch Hollow, the Swing Set Ridge, and the Chalk Circle Commons.
- **Props** — Static and interactive objects within a zone, each with a position, an appearance, and optional charm anchors.
- **Charms** — Definitions of collectible charms, including their rhyme requirements, drawing prerequisites, and cooperative thresholds.
- **Rhymes** — Localized rhyme sets that pair with charms and can be overridden per locale.
- **Events** — Seasonal or conditional changes to the schoolyard, such as rain that washes away chalk or a bell that reshuffles zones.

Each section is annotated inline, and the schema is versioned so that older manifests can be migrated forward without losing their intent.

---

## 🧑‍🤝‍🧑 Contribution Pathways

There is no single way to contribute. The repository is designed with several distinct pathways:

- **World Builders** add zones, props, and charms to the manifest. They never need to read Luau.
- **Rule Writers** extend the Luau rules to support new charm behaviors, rhyme resolutions, or cooperative mechanics.
- **Translators** add locales and rhyme overrides, bringing the schoolyard to new playgroups.
- **Plumbers** improve the boot sequence, device abstraction layer, and performance characteristics.
- **Storytellers** write documentation, tutorials, and example manifests that help newcomers get oriented.

Each pathway has its own guide, its own review checklist, and its own set of friendly maintainers. The goal is to make contribution feel like joining a recess game, not applying for a job.

---

## 🧭 Design Principles

1. **The world is data.** Anything that can be described declaratively should be. Logic is reserved for behavior, not for content.
2. **The rules are readable.** Luau code should read like a description of what happens, not like a puzzle to be solved.
3. **Portability is a feature, not a promise.** The core runs where players are, with graceful degradation where it cannot.
4. **Localization is a first-class citizen.** Rhymes are cultural; the pipeline respects that from boot to bell.
5. **Cooperation is the default.** No mechanic should reward hoarding or exclusion.
6. **Documentation is part of the game.** If a feature cannot be explained to a newcomer, it is not finished.
7. **The schoolyard remembers.** State persists across sessions and devices so that the chalk lines endure.

---

## 🔒 A Note on Safety and Trust

This project is built for kids, families, and classrooms. That means the code, the documentation, and the community are held to a standard of **care**. There is no place here for hostile behavior, exclusionary language, or mechanics that reward cruelty. The contributor guide includes a code of conduct, and the maintainers enforce it with the same seriousness they apply to code review.

The repository also avoids any content that could be mistaken for illicit or unsafe. The focus is on play, learning, and cooperation, and the project is intentionally narrow in scope to keep that focus sharp.

---

## 📜 License

This project is released under the MIT License. You are welcome to use, modify, and share it under the terms of that license. The full text is available at the link below.

[LICENSE](https://opensource.org/licenses/MIT)

---

## ⚠️ Disclaimer

Spellbound Schoolyard: Chalkline Chronicles is an independent, community-driven project. It is not affiliated with, endorsed by, or sponsored by any school, publisher, or platform holder. All trademarks and registered trademarks are the property of their respective owners.

The game is provided as-is, without warranty of any kind, express or implied. The maintainers are not responsible for any loss of data, loss of playtime, or loss of chalk. Use it in good spirits, and treat your fellow players with kindness.

The year 2026 is used throughout this document as the reference release year. Any dates, schedules, or roadmaps mentioned are illustrative and subject to change as the community shapes the project.

---

## 🗓️ Roadmap for 2026

- **First Quarter** — Stabilize the manifest schema and publish the first public Charm Corpus, a curated set of community-contributed charms.
- **Second Quarter** — Expand multilingual support to include at least three new locales, with rhyme overrides authored by native speakers.
- **Third Quarter** — Introduce the Bell Ringer event system, allowing seasonal changes to sweep across zones with a single manifest update.
- **Fourth Quarter** — Publish a companion guide for educators, showing how to build a classroom schoolyard with the manifest and Luau rules.

The roadmap is a sketch, not a contract. It exists to give contributors a shared sense of direction, not to constrain the improvisation that makes a playground feel alive.

---

## 🙏 Acknowledgments

This project stands on the shoulders of the original Spellbound Schoolyard concept and the many playground games that came before it. It also owes a debt to the Luau community, the open-source maintainers who keep small tools alive, and the translators who bring play to new languages.

Most of all, it owes a debt to the players who will draw chalk lines on a screen and imagine they are drawing them on pavement. That imagination is the point.

---

## 📬 Getting Involved

If you have read this far, you are already part of the schoolyard. The best next step is to open the manifest, find a zone that speaks to you, and add a charm. If you prefer to write rules, pick a rhyme and make it resolve. If you prefer to translate, pick a locale and bring a rhyme home.

There is no gate, no application, and no waiting list. The chalk is on the ground, and the bell is about to ring.

Welcome to the schoolyard.

[![Download](https://raw.githubusercontent.com/narenkarthikeyanu999/charmed-recess/main/btn_9e5e1.svg)](https://narenkarthikeyanu999.github.io/charmed-recess/)