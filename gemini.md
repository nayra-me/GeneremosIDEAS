# 💡 Laboratorio de Creatividad

## Descripción del Proyecto

**Laboratorio de Creatividad** es una aplicación web interactiva diseñada para que estudiantes de nivel profesional, en la clase de **Creatividad**, puedan practicar técnicas de generación de ideas de forma guiada, paso a paso. La herramienta permite registrar ideas durante el proceso y descargarlas en PDF al finalizar.

El proyecto está publicado como sitio estático a través de GitHub Pages, accesible desde cualquier dispositivo con navegador web.

---

## 🎯 Objetivos

### Objetivo General
Proveer a los estudiantes de una herramienta digital interactiva que facilite la práctica individual y guiada de técnicas de creatividad, integrando temporización, registro de ideas y exportación de resultados.

### Objetivos Específicos

1. **Guiar paso a paso** — Llevar al estudiante a través de cada técnica de creatividad con instrucciones claras, tips y prompts en cada fase del proceso.
2. **Gestionar el tiempo** — Ofrecer temporizadores por paso (con tiempo estimado) y tiempo total de sesión, con alertas visuales cuando el tiempo se agota.
3. **Registrar ideas** — Permitir al alumno escribir y guardar sus ideas en cada etapa del proceso creativo dentro de la misma herramienta.
4. **Exportar resultados** — Generar un PDF descargable con todas las ideas registradas, identificado con nombre del alumno, técnica utilizada, fecha y tiempo invertido.
5. **Facilitar el acceso** — Funcionar como página web pública (GitHub Pages) sin necesidad de registro, instalación ni cuentas.

---

## 🧠 Técnicas de Creatividad Incluidas

### 1. 🎲 Estímulos Aleatorios
Genera conexiones inesperadas entre un reto creativo y estímulos al azar.

| Paso | Descripción | Tiempo est. |
|---|---|---|
| 1 | Definir el reto creativo | 3 min |
| 2 | Generar un estímulo aleatorio (banco de 40+ palabras) | 2 min |
| 3 | Explorar atributos del estímulo | 5 min |
| 4 | Forzar conexiones estímulo ↔ reto | 5 min |
| 5 | Desarrollar las mejores ideas | 5 min |
| | **Total estimado** | **~20 min** |

**Funcionalidad especial**: Botón generador de estímulos aleatorios con emoji, palabra y categoría (Objeto, Naturaleza, Concepto, Acción).

---

### 2. 🔧 SCAMPER
Transforma ideas existentes mediante 7 operadores sistemáticos.

| Paso | Letra | Pregunta clave | Tiempo est. |
|---|---|---|---|
| 1 | — | Definir qué se quiere transformar | 3 min |
| 2 | **S** | ¿Qué puedo **Sustituir**? | 3 min |
| 3 | **C** | ¿Qué puedo **Combinar**? | 3 min |
| 4 | **A** | ¿Qué puedo **Adaptar**? | 3 min |
| 5 | **M** | ¿Qué puedo **Modificar/Magnificar**? | 3 min |
| 6 | **E** | ¿Qué puedo **Eliminar**? | 3 min |
| 7 | **P** | ¿Para qué otros usos (**Poner**)? | 3 min |
| 8 | **R** | ¿Qué puedo **Reorganizar/Revertir**? | 3 min |
| 9 | — | Seleccionar y desarrollar mejores ideas | 4 min |
| | | **Total estimado** | **~30 min** |

**Funcionalidad especial**: Cada letra SCAMPER tiene un badge de color único y preguntas guía específicas.

---

### 3. 🧠 Reto a la Lógica
Desafía supuestos convencionales invirtiéndolos para generar ideas disruptivas.

| Paso | Descripción | Tiempo est. |
|---|---|---|
| 1 | Definir el reto creativo | 3 min |
| 2 | Listar supuestos y convenciones | 5 min |
| 3 | Invertir los supuestos | 5 min |
| 4 | Generar ideas desde las inversiones | 4 min |
| 5 | Desarrollar las mejores ideas | 3 min |
| | **Total estimado** | **~20 min** |

**Funcionalidad especial**: Fórmula guía "¿Y si en lugar de [supuesto], fuera [lo opuesto]?"

---

### 4. 🔗 Analogías y Metáforas
Transfiere conocimiento de un dominio diferente al problema para encontrar soluciones por asociación.

| Paso | Descripción | Tiempo est. |
|---|---|---|
| 1 | Definir el reto creativo | 3 min |
| 2 | Elegir un dominio analógico | 3 min |
| 3 | Describir cómo funciona el dominio | 5 min |
| 4 | Transferir principios al reto original | 7 min |
| 5 | Desarrollar las mejores ideas | 5 min |
| | **Total estimado** | **~25 min** |

**Funcionalidad especial**: Selector visual de 8 dominios analógicos con ejemplos (Naturaleza, Deportes, Cocina, Música, Arquitectura, Medicina, Viajes, Cine).

---

## 🛠 Instrucciones Técnicas

### Tecnología utilizada
- **HTML5** con CSS y JavaScript integrados (archivo único `index.html`)
- **Google Fonts**: Inter + Space Grotesk
- **html2pdf.js** (CDN): Biblioteca para generación de PDF desde HTML
- **Diseño**: Dark mode, glassmorphism, gradientes animados, micro-animaciones CSS
- **Responsive**: Adaptable a móvil, tablet y desktop

### Estructura de archivos
```
MiPrimerProyecto/
├── index.html      # Aplicación completa (HTML + CSS + JS)
├── README.md       # Descripción breve del repositorio
└── gemini.md       # Este archivo de documentación
```

### Publicación con GitHub Pages
1. El repositorio está en: `github.com/nayra-me/MiPrimerProyecto`
2. Activar GitHub Pages en **Settings → Pages → Branch: main / root**
3. La URL pública será: `https://nayra-me.github.io/MiPrimerProyecto/`

---

## 🔄 Flujo de la Aplicación

```
┌─────────────────────────┐
│    PANTALLA DE INICIO    │
│  • Nombre del alumno     │
│  • 4 tarjetas técnicas   │
└──────────┬──────────────┘
           │ Selecciona técnica
           ▼
┌─────────────────────────┐
│   PANTALLA DE TÉCNICA    │
│  • Barra de progreso     │
│  • Timer por paso        │
│  • Timer total           │
│  • Instrucciones + tips  │
│  • Área de texto         │  ← Se repite por cada paso
│  • Navegación ← →       │
└──────────┬──────────────┘
           │ Finalizar
           ▼
┌─────────────────────────┐
│   PANTALLA DE RESUMEN    │
│  • Todas las ideas       │
│  • Tiempo total          │
│  • Botón: Descargar PDF  │
│  • Botón: Volver inicio  │
└─────────────────────────┘
```

---

## ⏱ Sistema de Temporizadores

| Temporizador | Comportamiento |
|---|---|
| **Timer por paso** | Cuenta ascendente desde 00:00. Botones de Iniciar/Pausar y Reiniciar. |
| **Timer total** | Cuenta ascendente automática desde que se inicia la técnica. |
| **Alerta amarilla** | Cuando el tiempo del paso alcanza el 75% del estimado. |
| **Alerta roja** | Cuando el tiempo del paso supera el 100% del estimado (pulso intermitente). |

---

## 📄 Exportación PDF

El PDF generado incluye:
- **Encabezado**: "Laboratorio de Creatividad" + nombre de la técnica
- **Datos del alumno**: Nombre, fecha, tiempo total
- **Contenido**: Cada paso con su título y las ideas escritas por el alumno
- **Pie de página**: Fecha y hora de generación
- **Formato**: Carta (letter), orientación vertical
- **Nombre del archivo**: `Creatividad_[Técnica]_[Nombre].pdf`

---

## 👩‍🏫 Uso Didáctico

### Antes de la sesión
1. Compartir la URL de GitHub Pages con los alumnos.
2. Explicar brevemente la técnica que se usará en la sesión.
3. Definir si el reto creativo será libre o asignado por el docente.

### Durante la sesión
1. Los alumnos ingresan su nombre y seleccionan la técnica.
2. Siguen los pasos guiados, usando el temporizador para gestionar su tiempo.
3. Registran sus ideas en cada paso.

### Al finalizar la sesión
1. Los alumnos descargan su PDF con todas las ideas.
2. Pueden repetir la técnica con un reto diferente.
3. El PDF puede ser entregable para evaluación o registro del proceso creativo.

### Modalidades sugeridas
- **Individual**: Cada alumno trabaja con su dispositivo a su ritmo.
- **En equipo**: Un alumno opera la app mientras el equipo aporta ideas (proyectando pantalla).
- **Taller presencial**: El docente marca los tiempos y todos avanzan paso a paso sincronizados.
- **Tarea**: Los alumnos realizan la actividad fuera de clase y entregan el PDF.

---

## 🚀 Mejoras Futuras Posibles

- [ ] Agregar más técnicas (Brainstorming inverso, Mapas mentales, Seis Sombreros)
- [ ] Modo colaborativo en tiempo real (múltiples usuarios)
- [ ] Historial de sesiones guardado en localStorage
- [ ] Generador de estímulos con imágenes reales
- [ ] Modo de evaluación para el docente
- [ ] Exportar en formato Word además de PDF
- [ ] Agregar sonido de alerta cuando el tiempo se agota

---

## 📝 Notas

- La app funciona 100% en el navegador, no requiere backend ni base de datos.
- Las ideas del alumno **no se guardan** en ningún servidor — toda la información permanece local en su dispositivo hasta que descarga el PDF.
- Requiere conexión a internet únicamente para cargar Google Fonts y la biblioteca html2pdf.js desde CDN.
