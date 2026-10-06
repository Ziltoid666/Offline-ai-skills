# Offline AI Skills

Personal skills for **Google AI Edge Gallery** and compatible Agent Skills implementations.

## Current skills

### `lew-local`

A text-only persona/behaviour skill for ordinary local-AI chat. It prioritises concise answers, accuracy, instruction-following, direct disagreement when warranted, dry humour when appropriate, and reduced conversational padding.

## Install in Google AI Edge Gallery

In **Agent Skills**:

1. Open the **Skills** manager.
2. Choose **Add skill**.
3. Use **Load skill from URL** if this repository is publicly hosted with GitHub Pages, or **Import local skill** if using the files directly on-device.
4. Point the loader at the skill folder, not directly at `SKILL.md`.

For `lew-local`, the hosted folder should end in:

```
/lew-local/
```

Google AI Edge Gallery expects this file to exist inside that folder:

```
lew-local/SKILL.md
```

## GitHub Pages

The repository includes an empty `.nojekyll` file so GitHub Pages serves `SKILL.md` as Markdown rather than processing it with Jekyll.

For URL loading, the files must be reachable by the phone without GitHub authentication. If the repository is private, use local import or make the hosted Pages output publicly accessible.

## Notes

A text-only skill is conditionally selected by the model from its name and description. If a behaviour must apply to **every single message without exception**, the app's System Prompt field is more deterministic. A persona skill is still useful because it is portable, shareable, and can coexist with more specialised skills.

Future candidates for this repository:

- auction/resale analysis;
- radio/shortwave logging;
- structured note extraction;
- API-backed lookup skills;
- interactive JavaScript/WebView tools;
- Android native-intent helpers where supported.
