# AGAIN — A voice on your shoulder

A shoulder-worn robotic assistant exploring when decision support is welcome during repeated shopping comparisons, and how a physical assistant can preserve the wearer’s control.

**[View the public portfolio](https://leviastudio925-collab.github.io/again-shoulder-assistant/)**

## Portfolio

Four current portfolio spreads, each 1684 × 595, are published in `assets/`:

1. Context, background, and research
2. Research evidence, behavioral measures, and design roadmap
3. Structure tests, prototyping, and technical framework
4. Application scenario, motion sequence, and evaluation plan

The webpage uses the project's navy palette and Libre Caslon Text. Open any spread to view it at full size.

## Prototype status

- **Existing physical demo:** ESP32, three SG90 servos, and printed mechanical parts; folded, raised, and retracted poses. The structure is adapted from an earlier project.
- **Planned integration:** camera video to computer-based MediaPipe tracking; Android test-page touch events; XiaoZhi-based voice service with Qwen; MCP tool requests for bounded ESP32 motion.
- **Prototype placeholders:** the current ultrasonic sensor and buzzer do not implement the proposed camera and microphone functions.
- **Evaluation pending:** comfort, endurance, movement repeatability, and usefulness of intervention timing.

Hand movement and timing variation are contextual cues, not proof of screen contact or indecision. The wearer is asked whether assistance is wanted.

This repository publishes the portfolio website and its visual assets. It does not contain working AI firmware or completed vision integration.

## Research

- [OpenStax, Calculus Volume 2, §3.7](https://openstax.org/books/calculus-volume-2/pages/3-7-improper-integrals): Gabriel's Horn as a mathematical metaphor.
- [Ferguson (1989), Who Solved the Secretary Problem?](https://doi.org/10.1214/ss/1177012493): stopping-rule assumptions and their limits.
- [Irie et al. (2022), Mental arithmetic modulates temporal variabilities of finger-tapping tasks in a tempo-dependent manner](https://doi.org/10.7717/peerj.13944).
- [Holm et al. (2017), Executive control and working memory are involved in sub-second repetitive motor timing](https://doi.org/10.1007/s00221-016-4839-6).

Portfolio research figures are qualitative summaries or illustrative schematics, not newly collected participant data. Transfer from laboratory tapping tasks to shopping hesitation remains a design hypothesis.

## Local viewing and deployment

Open `index.html` directly, or serve this directory with any static HTTP server. No build step or package installation is required.

GitHub Pages serves the repository root on the `main` branch. To update the gallery, replace the corresponding `assets/spread-0x.png` and push to `main`.

## Credits and rights

Libre Caslon Text is distributed under the SIL Open Font License; see [assets/OFL.txt](assets/OFL.txt). Public availability does not grant a license to reuse the portfolio artwork or photographs. Research sources are linked above.
