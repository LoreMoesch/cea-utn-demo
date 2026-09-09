# CEA-UTN · Prototipo del sistema de evaluación

Prototipo navegable del sistema de evaluación del Consejo Evaluador Académico (CEA) de la UTN.

**Ver la versión actual:** https://loremoesch.github.io/cea-utn-demo/

No requiere instalación: se abre en cualquier navegador.

---

## Versiones

| Versión | Link | Instrumento |
|---|---|---|
| **v5 (actual)** | [/](https://loremoesch.github.io/cea-utn-demo/) | Rúbrica de Evaluación de Aulas Virtuales en Carreras en Proceso de Implementación — **CEA 2026 VF2** |
| v4 (anterior) | [/v4.html](https://loremoesch.github.io/cea-utn-demo/v4.html) | Evaluación de carreras — 6 criterios / 27 indicadores, escala 1 a 4 |

## Instrumento vigente (VF2)

La unidad de evaluación es **el aula virtual de cada asignatura**. Las carreras agrupan sus aulas y el coordinador emite el dictamen a nivel carrera.

**13 criterios · escala 1 a 5 · máximo 65 puntos.**

### Escala de valoración

| Puntos | Nivel |
|---|---|
| 5 | Cumple plenamente |
| 4 | Cumple mayoritariamente |
| 3 | Cumple parcialmente |
| 2 | Cumple insuficientemente |
| 1 | No cumple |

Al evaluar, cada criterio muestra **el texto completo de los cinco descriptores** y el evaluador selecciona el nivel que corresponde.

### Los 13 criterios

1. Diseño, organización visual y navegación
2. Estructura general del aula virtual
3. Coherencia de los componentes didácticos
4. Objetivos y contenidos de enseñanza
5. Estrategias de enseñanza
6. Actividades de aprendizaje
7. Evaluación y retroalimentación
8. Organización temporal y cronograma
9. Uso pedagógico y pertinente del entorno virtual
10. Comunicación, interacción y acompañamiento
11. Accesibilidad e inclusión
12. Recursos y materiales didácticos
13. Diseño y potencialidad

### Valoración final (rangos orientativos, punto 5 de las notas)

| Rango | % de logro |
|---|---|
| Excelente | 90 – 100 % |
| Muy bueno | 80 – 89 % |
| Bueno | 70 – 79 % |
| Regular | 60 – 69 % |
| Desaprobado | menos de 60 % |

### Criterios críticos

Los criterios 1, 2, 3, 6, 7, 10 y 11 están señalados como críticos según el punto 6 de las notas metodológicas. El sistema avisa cuando alguno promedia 2,5 o menos, aunque el puntaje global sea alto.

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
