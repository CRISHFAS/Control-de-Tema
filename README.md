# 🌗 Sistema de Control de Tema Interactivo

Un sistema web ligero y elegante para ajustar la luminosidad de una página de forma gradual, implementado con tecnologías web fundamentales.

---

## ✨ Características

- **Interfaz Minimalista:** Un solo icono de sol/luna en la esquina superior derecha.  
- **Control Intuitivo:** Al hacer clic en el icono, aparece una barra de control vertical.  
- **Modo Gradual:** Ajusta la luminosidad de la página gradualmente, desde un **0% de oscuridad (modo claro)** hasta un **100% (modo oscuro)**.  
- **Interacción Rápida:** Puedes arrastrar el interruptor o hacer clic en cualquier parte de la barra para cambiar el tema al instante.  
- **Auto-Ocultamiento:** La barra de control desaparece automáticamente después de **3 segundos de inactividad**, manteniendo la interfaz limpia.  
- **Diseño Responsivo:** Se adapta y funciona en diferentes tamaños de pantalla.  

---

## 🛠️ Tecnologías Utilizadas

- **HTML:** Para la estructura semántica de la página.  
- **CSS:** Para el estilo y las transiciones fluidas. Se usan utilidades de **Tailwind CSS** para un desarrollo ágil y eficiente.  
- **JavaScript:** Para la lógica interactiva, el control de eventos y la manipulación del DOM.  

---

## 💡 Cómo Funciona

La magia detrás de este sistema reside en la combinación de **JavaScript y CSS**.

### 🔹 Lógica de Color
- JavaScript calcula el porcentaje de oscuridad (`darknessPercentage`) y lo usa para ajustar un valor de **luminosidad** en el color **HSL** del fondo (`hsl(210, 10%, [100-0]%)`).  
- Esto crea una transición suave entre el blanco y un tono de gris oscuro.  

### 🔹 Control de Eventos
- **Click en el botón del tema:** Alterna la visibilidad de la barra de control.  
- **Eventos `mousedown`, `mousemove` y `mouseup`:** Controlan la funcionalidad de arrastre del interruptor, permitiendo un ajuste **preciso y en tiempo real**.  
- **Click en la barra:** Ajusta el interruptor a esa posición de forma instantánea.  

### 🔹 Temporizador de Ocultamiento
- Se utiliza **`setTimeout`** y **`clearTimeout`** para gestionar un temporizador de **3 segundos** que oculta la barra automáticamente si no hay interacción.  
- Este temporizador se reinicia con cada acción, asegurando que el control no desaparezca mientras se está usando.  

---

## 🚀 Uso

1. Copia y pega el código completo en un archivo **`.html`**.  
2. Ejecútalo directamente en tu navegador.  

> ✅ No se requieren dependencias externas más allá de las librerías CSS y de iconos ya incluidas en el código.  

---

## 🎯 Ideal Para

Este proyecto es perfecto para aprender sobre:  

- Manipulación del **DOM**  
- Gestión de **eventos**  
- Creación de **interfaces de usuario interactivas** con tecnologías web fundamentales  
