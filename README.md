# Photo Second World

Turn a photograph into a minimal, connected paper-collage poster using a Codex skill.

## Concept

- One independent poster per uploaded photograph; never combine photos.
- Portrait 3:4 canvas, with equal photographic and paper halves.
- A shoreline, road, light beam, or other source structure continues across the midpoint into the paper world.
- Ivory paper, restrained collage, minimal black lines, and one short handwritten English caption.
- Optional tiny figures must interact with the continued structure, not serve as decoration.

## Install

Clone this repository into your Codex skills directory:

```sh
git clone https://github.com/robyboy888/photo-second-world.git ~/.codex/skills/photo-second-world
```

If that directory already exists, do not overwrite it blindly. Back it up or update its Git checkout. Start a new Codex chat if the skill is not discovered immediately.

## Use

Upload a photograph and ask:

```text
Use $photo-second-world to create a Second World poster from this photo.
```

For multiple photos, the skill creates separate posters. To get only a prompt, explicitly ask for a prompt without image generation.

## Requirements and limitations

This is an instruction skill, not a standalone image model. Actual rendering requires an image-editing tool available in the host, preferably Codex's built-in image generation. It includes no API credentials or paid-service integration. Availability and usage limits depend on the host.

The photographic region is instructed to retain identity, composition, lighting, and color, but generative editing cannot guarantee pixel-identical preservation. Check subject fidelity, the 3:4 ratio, the midpoint, physical continuity, and caption spelling before delivery.

Portrait source photos need proportional cropping to fit the upper 3:2 region. Originals must remain unchanged.

## Files

- `SKILL.md`: workflow and quality checks.
- `references/prompt-template.md`: reusable generation template.
- `agents/openai.yaml`: skill display metadata.

Private source photos and generated examples are intentionally excluded.
