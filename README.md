# AGAIN — A voice on your shoulder

A shoulder-worn robotic assistant exploring when decision support is welcome during repeated shopping comparisons, and how a physical assistant can preserve the wearer’s control.

**[View the public portfolio](https://leviastudio925-collab.github.io/again-shoulder-assistant/)**

## Portfolio

Four current portfolio spreads, each 1684 × 595, are published in `assets/`:

1. Context, background, and research
2. Research evidence, behavioral measures, and design roadmap
3. Finger-motion test, prototyping, and technical framework
4. Application scenario, motion sequence, and evaluation plan

The webpage uses the project's navy palette and Libre Caslon Text. Open any spread to view it at full size.

These four spreads were synchronized from the [Figma portfolio page](https://www.figma.com/design/ApoghdbZoRBlbBcDctaMXf/Untitled?node-id=96-160) on 12 October 2026.

## Prototype status

- **Existing physical demo:** ESP32, three SG90 servos, and printed mechanical parts; folded, raised, and retracted poses. The structure is adapted from an earlier project.
- **Completed hand-tracking test:** camera-based MediaPipe landmarks streamed to TouchDesigner, using index- and thumb-tip positions from both hands to explore tapping rhythm. The test uses coordinates, without calculating joint angles.
- **Planned integration:** hand-motion cues combined with Android test-page touch events; XiaoZhi-based voice service with Qwen; MCP tool requests for bounded ESP32 motion.
- **Prototype placeholders:** the current ultrasonic sensor and buzzer do not implement the proposed camera and microphone functions.
- **Evaluation pending:** comfort, endurance, movement repeatability, and usefulness of intervention timing.

Hand movement and timing variation are contextual cues, not proof of screen contact or indecision. The wearer is asked whether assistance is wanted.

This repository publishes the portfolio website and its visual assets. It does not contain the TouchDesigner project, firmware, or a working end-to-end AI integration.

## Finger-motion test and proposed assistance trigger

The active-tapping clip shows recurring movement cycles; the hesitation-labelled clip is less periodic. This is a preliminary qualitative observation, not a measured hesitation score or a validated classifier. The plotted traces were reconstructed from screenshots with individual vertical scales and an uncalibrated time axis, so they do not establish a numeric tapping frequency or a frequency-to-hesitation ratio.

A proposed next step counts valid movement cycles over a calibrated time window: **f = N / T**, where N is the number of cycles and T is the window duration in seconds. If the rate remains below a personally calibrated threshold for a set duration, with valid tracking and relevant task context, the arm would rise and ask whether assistance is welcome. The wearer could accept, decline, or stop; declining would return the arm to rest. No numeric threshold has yet been validated. Missing tracking should not trigger assistance.

## Research

- [OpenStax, Calculus Volume 2, §3.7](https://openstax.org/books/calculus-volume-2/pages/3-7-improper-integrals): Gabriel's Horn as a mathematical metaphor.
- [Ferguson (1989), Who Solved the Secretary Problem?](https://doi.org/10.1214/ss/1177012493): stopping-rule assumptions and their limits.
- [Irie et al. (2022), Mental arithmetic modulates temporal variabilities of finger-tapping tasks in a tempo-dependent manner](https://doi.org/10.7717/peerj.13944).
- [Holm et al. (2017), Executive control and working memory are involved in sub-second repetitive motor timing](https://doi.org/10.1007/s00221-016-4839-6).

The literature diagrams on spreads 1–2 are qualitative summaries or illustrative schematics, not newly collected participant data. The finger-motion plots on spread 3 illustrate this project's preliminary camera test and are traced from its screenshots. Transfer from laboratory tapping tasks to shopping hesitation remains a design hypothesis; a user study of assistance timing is still planned.

## Local viewing and deployment

Open `index.html` directly, or serve this directory with any static HTTP server. No build step or package installation is required.

GitHub Pages serves the repository root on the `main` branch. To update the gallery, replace the corresponding `assets/spread-0x.png` and push to `main`.

## Credits and rights

Libre Caslon Text is distributed under the SIL Open Font License; see [assets/OFL.txt](assets/OFL.txt). Public availability does not grant a license to reuse the portfolio artwork or photographs. Research sources are linked above.
