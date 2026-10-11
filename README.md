# docs_tesis

Repositorio agregador de los proyectos que componen el ecosistema de la tesis.
Los proyectos se mantienen como submodulos Git dentro de `submodules/`.

## Submodulos

| Ruta | Repositorio |
| --- | --- |
| `submodules/lerobot-vision-detector` | [dcuevasa/lerobot-vision-detector](https://github.com/dcuevasa/lerobot-vision-detector) |
| `submodules/lerobot-dataset-visualizer` | [dcuevasa/lerobot-dataset-visualizer](https://github.com/dcuevasa/lerobot-dataset-visualizer) |
| `submodules/lerobot_teleoperator_so101_ik` | [SinfonIAUniandes/lerobot_teleoperator_so101_ik](https://github.com/SinfonIAUniandes/lerobot_teleoperator_so101_ik) |
| `submodules/lerobot_robot_so101_mujoco` | [SinfonIAUniandes/lerobot_robot_so101_mujoco](https://github.com/SinfonIAUniandes/lerobot_robot_so101_mujoco) |
| `submodules/lerobot_teleoperator_so101_haptic` | [SinfonIAUniandes/lerobot_teleoperator_so101_haptic](https://github.com/SinfonIAUniandes/lerobot_teleoperator_so101_haptic) |
| `submodules/lerobot_teleoperator_so101_vuer` | [SinfonIAUniandes/lerobot_teleoperator_so101_vuer](https://github.com/SinfonIAUniandes/lerobot_teleoperator_so101_vuer) |

`FLAGlab/FLAG-Embodied-data`, mencionado en la wiki, queda pendiente de
acceso: GitHub responde `404/403` para la URL indicada. Cuando el repositorio
sea visible para la cuenta que clone este proyecto, se puede añadir con:

```bash
git submodule add https://github.com/FLAGlab/FLAG-Embodied-data.git submodules/FLAG-Embodied-data
```

## Clonar

Para clonar el agregador junto con todos sus proyectos:

```bash
git clone --recurse-submodules https://github.com/dcuevasa/docs_tesis.git
```

Si ya se clono el repositorio sin submodulos:

```bash
git submodule update --init --recursive
```

Para actualizar los submodulos a las ramas remotas configuradas:

```bash
git submodule update --remote --merge
```
