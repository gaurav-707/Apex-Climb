# Apex-Climb
# 🏎️ Apex Climb: Los Santos Exotics & Off-Road VI

[Play Live on Netlify](https://www.google.com/search?q=https%3A%2F%2Fdreamy-fudge-22904f.netlify.app%2F)
[GitHub Repo](https://www.google.com/search?q=https%3A%2F%2Fgithub.com%2Fgaurav-707%2FApex-Climb)
[Three.js r128](https://www.google.com/search?q=https%3A%2F%2Fthreejs.org%2F)
[Matter.js 0.19](https://www.google.com/search?q=https%3A%2F%2Fbrm.io%2Fmatter-js%2F)
[Web Audio API](https://www.google.com/search?q=https%3A%2F%2Fdeveloper.mozilla.org%2Fen-US%2Fdocs%2FWeb%2FAPI%2FWeb_Audio_API)

A self-contained 2.5D/3D Supercar & Off-Road Physics Racing Game built by **[@gaurav-707](https://www.google.com/search?q=https%3A%2F%2Fgithub.com%2Fgaurav-707)**. Engineered in a single zero-build HTML5 application combining **Three.js Physically Based Rendering (PBR)**, a **4x sub-stepped spring-damper suspension & rigid-body physics engine**, an **interactive Island Satellite Campaign Map**, and a **hybrid Web Audio API race-car sample & multi-harmonic V10/V12 synthesizer**.

## 🌐 Live Demo

- **Play Live in Browser**: [https://dreamy-fudge-22904f.netlify.app/](https://www.google.com/search?q=https%3A%2F%2Fdreamy-fudge-22904f.netlify.app%2F)
- **Source Repository**: [https://github.com/gaurav-707/Apex-Climb](https://www.google.com/search?q=https%3A%2F%2Fgithub.com%2Fgaurav-707%2FApex-Climb)

## ✨ Key Engineering Features

- **Sculpted Bezier `ExtrudeGeometry` 3D Vehicles**: Replaces primitive box meshes with contoured side-profile Bezier curves, wheel-arch cutouts, beveled body panels, sloped windshields, widebody fender flares, aerodynamic side mirrors, front splitters, rear diffusers with quad chrome exhaust tips, and 10-spoke concave alloy rims with slotted brake rotors and painted calipers.
- **Showroom PBR Shaders & Procedural HDR Reflections**: Uses `THREE.PMREMGenerator` to synthesize a real-time equirectangular studio and sky environment map applied across **Metallic**, **Pearlescent**, **Chrome**, and **Matte** paint finishes.
- **Stabilized 4x Sub-Stepped Physics & Nitro (`N2O`)**: Runs a 240 Hz sub-stepped suspension and tire traction solver with center-of-mass forward tangent Nitro thrust, automatic grounded pitch damping, and frame-rate-independent exponential chase camera smoothing (`50°–78°` dynamic FOV).
- **Real Race-Car Acceleration Audio + V10/V12 Harmonic Synth**: Decodes an embedded race-car acceleration recording via `AudioContext.decodeAudioData()`, dynamically modulating pitch and filter cutoff with live engine RPM, 7-speed Dual-Clutch (DCT) `70 ms` upshift cuts, twin-turbo spool whine, blow-off valve flutter, and decel exhaust crackles.
- **Interactive Satellite Island World Map**: Full-screen GPS mission selector featuring 6 distinct island biomes with automatic regional weather transitions (Bright Tropical Sun, Vice Golden Sunset, Wetlands Mist, Canyon Torrential Rainstorm with lightning and wet glossy road reflections, and Alpine Blizzard & Fog).
- **Articulated 3D Human Drivers & Spectators**: Hierarchical skeletal 3D character models for **Michael**, **Franklin**, and **Trevor** seated inside the cabin (turning the steering wheel and leaning with G-forces) and cheering along the track while waving and recording on smartphones.

## 🚘 Official Vehicle Roster (9 Models)

| Vehicle Model | Class | Drivetrain | Top Speed | Engine Layout | Price |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Ocelot F620** | Exotic Coupe | RWD / AWD | `275 KM/H` | Screaming V12 (`8,900 RPM`) | `$8,000` |
| **Benefactor Schwartzer** | Sports Coupe | AWD | `270 KM/H` | Twin-Turbo V10 (`8,600 RPM`) | `$8,000` |
| **Übermacht Sentinel XS** | Tuner Coupe | AWD | `248 KM/H` | High-Revving V8 (`8,400 RPM`) | `$6,000` |
| **Lampadati Felon GT** | Grand Tourer | AWD | `282 KM/H` | Italian Exotic V12 (`9,000 RPM`) | `$9,500` |
| **Gallivanter Baller** | Luxury SUV | 4WD | `228 KM/H` | Supercharged V8 (`7,400 RPM`) | `$9,000` |
| **Obey Rocoto** | Sport SUV | AWD | `235 KM/H` | Rally Raid V10 (`7,600 RPM`) | `$8,500` |
| **Mammoth Patriot** | Heavy Humvee | 4WD | `192 KM/H` | Heavy-Duty V8 (`6,600 RPM`) | `$5,000` |
| **Vapid Sandking XL** | Lifted 4x4 XL | 4WD | `198 KM/H` | Monster Torque V8 (`6,800 RPM`) | `$4,500` |
| **Vapid Sandking SWB** | Lifted 4x4 SWB | 4WD | `204 KM/H` | Baja Spec V8 (`6,900 RPM`) | `$4,500` |

## 🗺️ Island Campaign Regions & Interactive Physics Set-Pieces

| Region | Location Name | Default Weather | Distance | Payout | Signature Physics Set-Pieces |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Region 1** | **Southern Tropical Keys** | Bright Tropical Sun | `560 m` | `$2,000` | Turquoise ocean causeways, palm beaches, and island wooden ramp jumps |
| **Region 2** | **Vice Beach & East Coast City** | Vice Golden Sunset | `680 m` | `$2,800` | Neon coastal boulevards and tall collapsible brick/steel wall bridges over chasms |
| **Region 3** | **Grassrivers Lake & Wetlands** | Wetlands Humid Mist | `740 m` | `$3,600` | Muddy high-drag swamp trails, stilt villages, and timber tower bridges |
| **Region 4** | **West Coast Port & Highway** | Vice Golden Sunset | `820 m` | `$4,500` | Pivoting seesaw bridges balanced on central fulcrums and breakable barricades |
| **Region 5** | **Northwest Mountain Canyon** | Torrential Canyon Storm | `900 m` | `$6,000` | Wet glossy rock (`roughness: 0.08`), lightning flashes, boulder traps, and N2O canyon jumps |
| **Region 6** | **Northern Alpine Summit** | Alpine Blizzard & Fog | `1,020 m` | `$8,500` | Icy low-friction ledges, collapsible wall bridges, seesaws, and summit N2O jump gauntlet |

## 🎮 Controls

| Control / Input | Ground Action | Mid-Air / UI Action |
| :--- | :--- | :--- |
| `D` / `Right Arrow` / **THROTTLE** | Accelerate forward | Pitch nose-up (Wheelie / Backflip) |
| `A` / `Left Arrow` / **BRAKE** | Hydraulic disc brakes & reverse | Pitch nose-down (Leveling / Frontflip) |
| `Shift` / `Space` / `W` / **N2O PURGE** | Inject stabilized center-of-mass Nitrous Oxide | Mid-air forward jet boost |
| `M` | Open Interactive Island Satellite Map | Select region & view GPS telemetry |
| `G` / `Esc` | Return to Luxury Autos Showroom & Mod Bay | Orbit 3D turntable & customize vehicle |
| `R` | Instant stage retry | Restart current region |

## 🛠️ Local Development & Deployment

Because the entire game is self-contained inside `index.html`, no build step or bundler is required:

```bash
# Clone the repository
git clone https://github.com/gaurav-707/Apex-Climb.git
cd Apex-Climb

# Option 1: Open index.html directly in any browser
open index.html

# Option 2: Run a local static server
npx serve .
```

## 📄 License

Released under the **MIT License** by [@gaurav-707](https://www.google.com/search?q=https%3A%2F%2Fgithub.com%2Fgaurav-707).
