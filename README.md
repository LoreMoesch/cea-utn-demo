# CEA-UTN · Prototipo del sistema de evaluación

Prototipo navegable del sistema de evaluación del Consejo Evaluador Académico (CEA) de la UTN.

**Ver la versión actual:** https://loremoesch.github.io/cea-utn-demo/

No requiere instalación: se abre en cualquier navegador.

---

## Versiones

| Versión | Link | Instrumento |
|---|---|---|
| **v5 (actual)** | [/](https://loremoesch.github.io/cea-utn-demo/) | Rúbrica de Evaluación del Aula Virtual — CEA 2026 |
| v4 (anterior) | [/v4.html](https://loremoesch.github.io/cea-utn-demo/v4.html) | Evaluación de carreras — 6 criterios / 27 indicadores |

## Qué cambió en la v5

La rúbrica aprobada por el CEA en 2026 cambió la unidad de evaluación y la escala:

- **Unidad evaluada:** ahora es el **aula virtual de cada asignatura**, no la carrera. Se agregó la jerarquía Carrera → Asignatura → Aula.
- **Instrumento:** 13 criterios planos (antes 6 criterios con 27 indicadores).
- **Escala:** 1 a 5 — Excelente (5), Muy bueno (4), Bueno (3), Regular (2), Desaprobado (1). Antes era 1 a 4.
- **Resultado:** puntaje sobre **65 puntos**, porcentaje de logro (puntaje ÷ 65 × 100) y valoración final por rangos.
- Al evaluar, cada criterio muestra **el texto completo de los cinco descriptores** de la rúbrica; el evaluador selecciona el nivel que corresponde.
- **Criterios críticos** (§6 de las notas metodológicas: 1, 2, 3, 6, 7, 10, 11) señalados, con alerta cuando alguno promedia ≤ 2,5 aunque el puntaje global sea alto.

### Rangos de valoración final

| Rango | % de logro |
|---|---|
| Excelente | 90 – 100 % |
| Muy bueno | 80 – 89 % |
| Bueno | 70 – 79 % |
| Regular | 60 – 69 % |
| Desaprobado | menos de 60 % |

## Accesos de demostración

| Rol | Usuario (DNI) | Contraseña |
|---|---|---|
| Administrador | 20111111 | admin2026 |
| Coordinador | 20222222 | coord2026 |
| Evaluador/a | 20333333 · 20444444 · 20555555 | cea2026 |

Son credenciales ficticias de demostración, sin valor fuera de este prototipo.

## Alcance

Es un **prototipo de interfaz** para validar el instrumento y los circuitos de trabajo con el CEA antes de construir el sistema:

- Los datos **no se guardan**: viven en memoria y se pierden al recargar la página.
- Los mails de notificación se **simulan** (quedan registrados en Reportes → Log de notificaciones).
- La carga de archivos registra el nombre, no sube el contenido.

Autenticación real, base de datos, envío de correo por el relay institucional y despliegue son parte de la etapa siguiente.
