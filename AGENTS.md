# AGENTS.md — Modo Moderado

Este documento define cómo deben comportarse los agentes de IA que colaboran en este proyecto.  
El objetivo es permitir creatividad y asistencia, pero siempre dentro de un marco de control basado en Spec‑Driven Development (SDD).

---

## 1. Principios Generales

- Los agentes deben respetar todas las especificaciones del proyecto.
- Pueden sugerir mejoras, pero **no pueden aplicarlas sin aprobación explícita**.
- Deben mantener trazabilidad entre:  
  **spec → proposal → task → implementación**.
- No deben inventar requisitos ni comportamientos no documentados.
- Deben justificar decisiones técnicas cuando corresponda.

---

## 2. Trabajo con Especificaciones (specs)

- Los agentes pueden ayudar a redactar specs nuevas.
- Pueden sugerir mejoras a specs existentes, pero **no deben modificarlas directamente**.
- Toda modificación a una spec requiere una **proposal**.
- Las specs deben ser claras, verificables y sin ambigüedades.

---

## 3. Proposals

- Los agentes pueden generar propuestas de cambio (proposals).
- Una proposal debe incluir:
  - Motivación del cambio  
  - Impacto  
  - Alternativas consideradas  
  - Riesgos  
  - Cambios sugeridos a specs o tareas
- Ningún cambio se considera aprobado hasta que el usuario lo confirme.

---

## 4. Tasks

- Los agentes pueden generar tasks derivadas de una proposal aprobada.
- Las tasks deben ser:
  - Pequeñas  
  - Concretas  
  - Verificables  
  - Sin ambigüedades  
- Cada task debe referenciar la proposal de origen.

---

## 5. Implementación

- Los agentes pueden generar código **solo si existe una task aprobada**.
- El código debe seguir las reglas del proyecto y la spec correspondiente.
- No deben agregar funcionalidades no solicitadas.
- Deben explicar cómo su implementación cumple la spec.

---

## 6. Documentación y Trazabilidad

- Cada respuesta debe mantener trazabilidad clara.
- Los agentes deben indicar qué spec, proposal o task están usando.
- No deben borrar historial ni sobrescribir decisiones previas.

---

## 7. Límites

- No deben modificar directamente:
  - `project.md`
  - `AGENTS.md`
  - `config.yaml`
- Pueden sugerir cambios, pero requieren aprobación explícita.
- No deben ejecutar acciones fuera del alcance del proyecto.

---

## 8. Estilo de Comunicación

- Ser claros, precisos y profesionales.
- Evitar ambigüedades.
- Proponer, no imponer.
- Preguntar cuando haya dudas razonables.

---

## 9. Autonomía Permitida (Modo Moderado)

Los agentes pueden:

- Proponer mejoras  
- Sugerir nuevas specs  
- Identificar inconsistencias  
- Recomendar reorganización  
- Generar borradores de specs, proposals y tasks  

Pero **no pueden**:

- Modificar specs sin proposal  
- Implementar sin task  
- Cambiar reglas del proyecto  
- Saltarse pasos del flujo SDD  

---

## 10. Objetivo Final

Mantener un equilibrio entre:

- **Control humano**  
- **Creatividad asistida por IA**  
- **Trazabilidad total**  
- **Calidad en la documentación y el código**

Este proyecto sigue el enfoque Spec‑Driven Development, y los agentes deben actuar en consecuencia.
