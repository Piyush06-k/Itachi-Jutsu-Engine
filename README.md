# Itachi-Jutsu-Engine


An interactive, high-fidelity web application that visualizes classic Naruto ninjutsu and genjutsu using advanced browser graphics and real-time computer vision. Named after Itachi Uchiha, this application simulates various chakra states and visual techniques utilizing a robust 3D particle system combined with optional MediaPipe hand-gesture tracking.


## 👁️ Project Overview
The Itachi Jutsu Engine uses the power of modern web technologies to bring anime visual effects to life in a browser. By either utilizing your computer's webcam or an on-screen manual deck, you can trigger complex, morphing particle architectures that mimic legendary Uchiha techniques.


### Core Features
* High-Fidelity Particle System: Animates 25,000 active particles with unique color gradients, sizes, and physics algorithms per technique.
* AI Hand Tracking: Leverages Google MediaPipe to actively scan and interpret hand formations in real-time.
* Cinematic Post-Processing: Built with Three.js EffectComposer incorporating heavy bloom effects, custom fog, and a film grain shader.
* Responsive Control Deck: A fully optimized overlay panel allows users without webcams to seamlessly experience all visual states.


## 🎛️ Jutsu Deck & Technical Specifications

The particle engine transitions smoothly between five distinct chakra states using custom mathematical coordinate mappings calculated on the fly:

| # | Technique Name | Visual Behavior & Particle Dynamics | Mathematical Blueprint | Hand Seal Trigger |
| :--- | :--- | :--- | :--- | :--- |
| **1** | **Chakra Neutral State** | Calm, orbiting ash cloud mixed with a quiet background mist. Silent and idle. | Random spherical orbital distribution with a slow, stabilizing $y$-axis rotation. | **Default state** / No hands detected.|
| **2** | **Tiger Seal: Fire Ball Jutsu** | A roaring, rapidly rising flame tornado. Particles glow with a bright fiery gradient (orange to neon gold). | Dynamic expanding cone vortex stretching upwards along the $y$-axis with rapid rotation. | **Tiger Seal** (Both hands raised up close together). |
| **3** | **Illusion: Genjutsu Anime Seal** | An intense, vibrating visual circle consisting of a glowing kanji symbol, a pentagram star, and outer power rays. | Precomputed pentagram vertices, linear stroke segment mapping for the Kanji **"幻"**, and high-frequency noise vibration. | **Genjutsu Finger** (Only the index finger raised straight up). |
| **4** | **Mangekyō Sharingan Activated** | Itachi’s signature three-bladed ocular pinwheel. Features a pitch-black pupil core and a heavy outer bounding ring. | Logarithmic spiral segment progression formulas ($r = a \cdot e^{b\theta}$) rotating rapidly on a fixed flat 2D plane. | **Akatsuki Pose** (Thumb and index finger pinched closely together). |





