# nex

![3d side](content/3dside.png)

**nex** is a swarm robotics project built around **ESP32-based bots**, computer vision, AprilTags, and a custom 4-layer PCB. The goal is to have multiple small bots identify and communicate with each other while working together as a swarm.

it features:

- ESP32-WROOM in each bot for wireless communication
- Luckfox Lyra Zero W for computer vision
- AprilTags for identifying individual bots
- Custom 4-layer PCB designed in KiCad

## how it works

each bot has an **ESP32-WROOM** which handles communication between the bots and provides the wireless connection. Each bot also has its own AprilTag, giving the vision system a way to identify which bot it is looking at.

the **Luckfox Lyra Zero W** handles the computer vision side. It detects the AprilTags and uses their position and orientation to work out where the other bots are.

this allows the bots to know who is around them and where they are, which forms the basis for the swarm behaviour.

## KiCad

the electronics are built around a custom **4-layer PCB**, designed to keep the different parts of the bot connected without needing a large amount of external wiring.

|              schematic              |           PCB           |
| :---------------------------------: | :---------------------: |
| ![schematic](content/schematic.png) | ![PCB](content/pcb.png) |

|        PCB mockup top         |          PCB mockup bottom          |
| :---------------------------: | :---------------------------------: |
| ![top](content/3dpcb_top.png) | ![bottom](content/3dpcb_bottom.png) |

## Fusion

the mechanical design and overall bot layout were modelled in Fusion.

|             top              |              side              |               bottom               |
| :--------------------------: | :----------------------------: | :--------------------------------: |
| ![3d top](content/3dtop.png) | ![3d side](content/3dside.png) | ![3d bottom](content/3dbottom.png) |

## BOM

the complete bill of materials is available in [`bom.csv`](bom.csv).

## firmware

firmware is not included yet. The software will be added after the physical bots are built and the hardware can be tested and debugged.
