# docs_tesis

Este repositorio reúne como submódulos Git los proyectos que forman parte del
ecosistema de la tesis. La descripción técnica y la relación entre los
proyectos se encuentra en la [wiki del proyecto](https://github.com/dcuevasa/docs_tesis/wiki).

## Inicialización

Para clonar el repositorio junto con todos sus submódulos:

```bash
git clone --recurse-submodules https://github.com/dcuevasa/docs_tesis.git
```

Si el repositorio ya fue clonado sin submódulos, inicialízalos con:

```bash
git submodule update --init --recursive
```

## Arquitectura de Modelo: `lerobot_policy_modular_vla`

Contiene la implementación plug-and-play del modelo modular para LeRobot ("AI MODEL" entre comillas):
* **Orquestador VLM:** Planificador configurable con soporte para Ollama (local), OpenAI, Gemini, Claude, transformers o Mock.
* **Aislamiento Visual:** Acondicionamiento mediante recortes (*crops*), máscaras o *bounding boxes* para desacoplar el razonamiento semántico del control motor.
* **Micro-Expertos & Model Swapping:** Gestión de micro-modelos (ACT, Diffusion, etc.) con estrategia de intercambio dinámico de baja VRAM y opción de conmutación CORAL (cabezales LoRA).
* **Superposición Visual:** Grabación directa de *bounding boxes* y HUD informativo sobre los videos de telemetría y evaluación.

Para más detalles, consulta la documentación en [`lerobot_policy_modular_vla/README.md`](lerobot_policy_modular_vla/README.md).
