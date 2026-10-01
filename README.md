# Know Your Farm

An interactive dashboard of Indonesian farmer and livestock groups (kelompok tani, kelompok ternak, gabungan kelompok tani) found through **public Instagram profiles**.

**Live dashboard:** https://lbharoto.github.io/Know-your-Farm/

## What you can see

- **Group type, commodity and region** for each group
- **Activity:** how recently a group posted, plus its reach and engagement
- **Responsible KPwDN office** for the group's regency or city
- **Likely needs:** items from the incentive catalogue the group may be able to use
- A searchable, sortable table. Click a row for the group's summary, evidence and a link to its Instagram profile

Use the filters at the top, or click any bar or column in the charts, to narrow the list.

## How the data was made

1. Instagram profiles were found by keyword search ("kelompok tani", "gapoktan", "poktan", "peternak" and similar) and collected with Apify.
2. An AI model read each bio and the newest posts to classify the group, identify its location, and suggest likely needs from a fixed item list.
3. Each group's regency was matched to the responsible KPwDN office using the official coverage list.

## Please read before relying on this

- **The AI output is a lead, not a fact.** Group type, region, KPwDN office and especially the likely needs are suggestions. Most needs are inferred from the commodity, not stated by the group. Verify with the group before acting.
- **Member counts are placeholders.** Instagram rarely states them, so the Members column uses a default guess by group type, marked "est.". Land area is almost always empty. Do not use either for sizing decisions.
- Some groups have no KPwDN office because their profile names no location.
- Only groups judged relevant are included. The classification can be wrong.

## Privacy

- All profiles are **public**. Phone numbers, email addresses, WhatsApp links and contact fields were **removed** from this public version.
- If you run one of these accounts and want it taken off this page, open an issue with your Instagram username and it will be removed.

## Files

- `index.html`: the whole dashboard in one self-contained file (data included). No server needed.
