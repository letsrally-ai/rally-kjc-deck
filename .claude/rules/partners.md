# Adding a New Partner

Follow this pattern every time a new partner is pitched in the deck.

## 1. Tab button
In `#ptabs` (inside the Partnership slide, `<div id="s7">`), append:
```html
<div class="ptab" onclick="pt('<id>',this)">Partner Name</div>
```

## 2. Content panel
Add a panel after the last `.pc` block, mirroring the structure of `#pc-kjcba` / `#pc-ali` / `#pc-any`:
```html
<div class="pc" id="pc-<id>">
  <div class="pl">
    <div class="pi-box">  <!-- eyebrow + h3 + intro + .bl benefits --> </div>
    <div><div class="ask-box"> <!-- h5 + .ai.xl asks --> </div></div>
  </div>
</div>
```

## 3. Slide visibility
Append `<id>` to the `data-partners` attribute on every partner-gated slide (currently `#s6`). Do not touch slides with `data-partners="all"`.

## 4. URL-param wiring
In the `<script>` block (~lines 2382–2392), add the partner to both maps:
```js
PARTNER_NAMES: { ..., <id>: 'A Proposal for <Partner Name>' }
PARTNER_TAB:   { ..., <id>: '<tabId>' }  // tabId matches the pt() call in step 1
```

## 5. Verify
- Internal view (`index.html`): new tab renders, switches content, animates in.
- Partner view (`index.html?p=<id>`): tab bar is hidden, partner's panel is active by default, non-partner slides are hidden, counter is accurate.
- Regression: every other `?p=` URL still works unchanged.

## Ids in use
- `kjcba` → KJCBA (tabId `kjcba`)
- `alibabar` → Alibabar (tabId `ali`)
- `anywheel` → Anywheel (tabId `any`)
- `grab` → Grab Holdings (tabId `grab`)
