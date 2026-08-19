# nex

esp32 based swarm bots based on cv, apriltags and a custom 4 layer pcb.

## design

there's an esp32 wroom in each bot which is used to connect to the bots and for the bots to connect to each other. each bot will have april tags mounted on them which will be used to identify them using cv on the luckfox lyra zero w. firmware and code will be added once the project is built and i can debug and confirm it all runs.

### kicad

|              schematic              |           pcb           |
| :---------------------------------: | :---------------------: |
| ![schematic](content/schematic.png) | ![pcb](content/pcb.png) |

|        pcb mockup top         |          pcb mockup bottom          |
| :---------------------------: | :---------------------------------: |
| ![top](content/3dpcb_top.png) | ![bottom](content/3dpcb_bottom.png) |

### fusion

|             top             |             side              |              bottom               |
| :-------------------------: | :---------------------------: | :-------------------------------: |
| ![3dtop](content/3dtop.png) | ![3dside](content/3dside.png) | ![3dbottom](content/3dbottom.png) |

## bom

click [here](bom.csv) for the bom.

## firmware

not yet, will be done once I've made the nex bots irl
