# 🌾 Kisan Saathi

**A crop-loss claim assistant for Marathwada farmers, built with Genspark Super Agent at Genspark Pune Meetup (4 Oct 2026).**

## Problem

El Niño dry spells, water shortage and sudden heavy rain keep hitting farmers in Marathwada,
Maharashtra (Beed, Latur, Jalna, Nanded, Parbhani, Hingoli, Dharashiv, Chhatrapati Sambhajinagar).
Many lose crop-insurance (PMFBY) claims because they:

- don't know about the **72-hour** reporting window for floods, hail and other localised calamities,
- don't know which documents and photos are needed,
- don't know that **drought is handled differently** — it is assessed for the whole area, so there is no 72-hour rule.

## Solution

Kisan Saathi turns "my crop is gone" into a ready claim kit in under a minute, in **Marathi, Hindi or English**:

1. Collects the farmer's details (district, crop, acres, what happened, when, PMFBY status).
2. Picks the right path:
   - 🔴 **URGENT** — flood / hail / cloudburst under 72 hours: report now on helpline **14447** or the Crop Insurance app.
   - 🟠 **Late** — over 72 hours: honest next-best steps (agriculture office, bank, panchanama / girdawari).
   - 🔵 **Drought / pest** — area-based assessment: keep enrolment active, e-Pik Pahani entry, weekly dated photos, ask about drought declaration.
3. Builds a claim kit: document checklist, photo instructions, and a ready-to-send message (copy or WhatsApp).
4. Explains what happens next — without promising any amount or timeline.

**Safety rules:** never states a compensation amount as current or guaranteed; always tells the farmer to confirm with their district / taluka agriculture office.

## What's in this repo

| File | What it is |
|---|---|
| [`GENSPARK_SUPER_AGENT_PROMPT.md`](GENSPARK_SUPER_AGENT_PROMPT.md) | The Kisan Saathi prompt for Genspark Super Agent, test inputs, and 2-minute pitch |
| [`index.html`](index.html) | Offline web app — one file, no server, no API key. Open it in any browser. |
| [`screenshots/`](screenshots) | Demo screenshots: the app (Marathi drought case) and Genspark Super Agent (Hindi flood URGENT case) |

## Run it

Open `index.html` in a browser and click **डेमो भरा / Fill demo** → **Make my claim kit**.

## Built with Genspark Super Agent

The prompt was tested live in Genspark Super Agent:

- **Marathi drought case** (Beed, soybean) → correctly said the 72-hour rule doesn't apply, gave the claim kit and Marathi message.
- **Hindi flood case** (Latur, tur) → opened with "⚠️ ज़रूरी और तुरंत — 72 घंटे की समय-सीमा चल रही है", checked the current time to count hours.

## Next steps

- WhatsApp and voice-call version for farmers who can't type (Marathi voice agent).
- Live data: district drought declarations and mid-season adversity notifications.

> ⚠️ Kisan Saathi is a helper, not official advice. Scheme rules and amounts vary by state, crop, season and year. Always confirm with your district agriculture office.
