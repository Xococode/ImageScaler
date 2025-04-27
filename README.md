# Image Scaler & Adjuster

Una aplicación web para escalar imágenes con interpolación bicúbica y ajustar brillo, contraste, nitidez, tono y saturación en tiempo real, con comparador deslizable y soporte de zoom/paneo.

---

## Acceso rápido a la aplicación 🚀
👉 [**Probar en vivo aquí**](https://xococode.github.io/ImageScaler/)

---

## 🧭 Navegación y control de vista

- **Zoom**  
  - Rueda del ratón sobre la imagen comparada (área principal)  
  - Límite: desde 1× hasta 10×  
- **Paneo (mover imagen)**  
  - Clic izquierdo y arrastrar cuando el zoom está por encima de 1×  
  - Cursor cambia a “grab” / “grabbing”

---

## 🚀 Flujo de uso

1. ### Cargar imagen  
   - Haz clic en **Select Image** o arrastra/pega tu imagen en el área principal.  
   - Soporta formatos comunes (`.png`, `.jpg`, `.jpeg`, etc.).

2. ### Configurar parámetros  
   - **Scale Factor**: factor de escalado (1×–16×).  
   - **Sharpen**: controla cuánto afilar (0–3).  
   - **Brightness**: brillo (-50% a +50%).  
   - **Contrast**: contraste (50% a 150%).  
   - **Hue Rotation**: giro de matiz (-180° a +180°).  
   - **Saturation**: saturación (0% a 200%).  
   - Los valores se muestran al lado de cada control.

3. ### Procesar imagen  
   - Pulsa **Scale & Adjust**.  
   - Verás una barra de progreso y mensajes de estado.

4. ### Comparar antes/después  
   - Usa el deslizador (`img-comparison-slider`) para ver la diferencia entre original y procesada.

5. ### Salida y descarga  
   - Tras completar, habilita botones para:
     - **Download PNG**: descarga la imagen procesada.  
     - **Copy Image**: copia directamente al portapapeles (si el navegador lo permite).

6. ### Reset  
   - Haz clic en el botón **Reset** (↺) para volver al estado inicial y parámetros por defecto.

---

## ⚙️ Atajos y consejos

- **Guardar parámetros**: no aplica, la configuración se renueva al recargar.  
- **Reset rápido**: botón superior derecho “↺”.  
- **Arrastrar y soltar**: compatible con drag & drop y pegado (`Ctrl + V`).  
- **Interfaz responsiva**: se adapta al tamaño del área de contenido.

---

## ✅ Ventajas

- **Sin necesidad de instalar**: funciona en el navegador.  
- **Procesamiento en cliente**: tu imagen nunca sale de tu equipo.  
- **Alta calidad**: interpolación bicúbica + ajustes suaves.  
- **Comparador incorporado**: ve al instante el “antes” y “después”.  
- **Zoom y paneo**: explora detalles en alta resolución.  
- **Soporte de portapapeles**: copia directamente sin descargar.

---

## 📂 Estructura de archivos

- **`index.html`**: interfaz y estilos.  
- **`<script>`** interno:
  - Lectura y renderizado de imagen en `<canvas>`.  
  - Algoritmos de bicúbica, nitidez, brillo/contraste, HSL.  
  - Manejo de UI (progreso, estado, habilitación de botones).  
  - Lógica de zoom/paneo sobre el wrapper.

---

¡Disfruta escalando y ajustando tus imágenes de forma interactiva!  
