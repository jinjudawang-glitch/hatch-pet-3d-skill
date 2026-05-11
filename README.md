# Hatch Pet 3D Skill

A Codex skill for creating 3D-style animated desktop pets.

This is a modified version of `hatch-pet`.  
The original workflow is kept: it generates a Codex-compatible pet spritesheet, validates the frames, creates QA contact sheets, and packages the final pet.

The main change is the default style.

Instead of pixel-style pets, this version is tuned for compact 3D desktop companions: soft toy-like proportions, oversized heads, readable silhouettes, soft fur or fabric materials, and small expressive motions.

## What It Does

This skill helps generate a Codex-compatible animated pet from a concept or reference image.

It can:

- create a base pet design
- generate animation rows for different states
- keep the pet identity consistent across frames
- split and align animation frames
- assemble the final spritesheet
- validate the atlas
- package the pet for Codex

## Animation States

The generated spritesheet follows the Codex pet format:

| Row | State |
| --- | --- |
| 0 | idle |
| 1 | running-right |
| 2 | running-left |
| 3 | waving |
| 4 | jumping |
| 5 | failed |
| 6 | waiting |
| 7 | running |
| 8 | review |

Each row is one state.  
Each cell is one animation frame.

## 3D Pet Style

This version is designed for 3D desktop pets.

The default prompt style asks for:

- compact full-body 3D pet sprites
- soft toy-like proportions
- slightly oversized heads
- rounded limbs
- simple expressive faces
- clean studio lighting
- simplified fur, fabric, eyes, collars, bows, or accessories
- details that remain readable at 192x208

It avoids:

- pixel art
- thick pixel outlines
- flat 2D sticker art
- photorealistic animal portraits
- overly detailed fur
- glossy app-icon style images

## Better Motion Prompts

One important change is how actions are described.

For example, waving should not only move one paw.  
The pet should also have small supporting motions:

- head tilt
- eye change
- mouth change
- ear movement
