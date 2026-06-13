# Casa-SM Interactive Electrical Design & Simulation Software

An interactive, web-based CAD tool specifically designed for visualizing, mapping, and testing the electrical layout of the **Casa-SM** residential project. Built purely with modern web technologies, it allows users to overlay dynamic electrical circuits directly onto architectural blueprints, bundle wall switches into modular vertical boxes, and test configurations using a live grid simulation mode.

## 🚀 Live Demo

You can run and test this application directly from your browser without installing anything:
👉 **[LAUNCH LIVE APP](https://santimaldonado2.github.io/electrodesign/)** *(Replace with your actual GitHub Pages link once enabled)*

---

## ✨ Features

- **Dynamic Blueprint Mapping:** Precision point-and-click placement of components aligned to the underlying scale of architectural plans (`IE_01`).
- **Diverse Luminarie Subtypes:** Fully supports 3 distinct lighting modules with custom spatial representations:
  - 💡 **Standard Lights:** Circular residential general-purpose overhead outlets.
  - 🔳 **Floodlights/Reflectors:** Squared exterior projectors featuring targeted high-intensity lighting beams.
  - ➖/🪟 **LED Light Strips:** Directional linear modules configurable in either **Horizontal** or **Vertical** orientations.
- **Smart Modular Switch Boxes (Cambre/Sica Style):** Clean up blueprint clutter by multi-selecting (`CTRL` + Click) overlapping wall switches and grouping them into sleek, compact vertical wall faceplates.
- **Live Energy Simulation Mode:** Activate the grid to toggle power distribution. Grouped switch plates display independent live feedback—individual keys dynamically switch to green when their connected sub-circuit is powered.
- **Dynamic Deconstruct Feature:** Mistakenly grouped a box? A simple **Right-Click** disassembles any modular faceplate, resetting switches back to their exact original layout positions.
- **JSON Project Version Control:** Full **Export** and **Import** functionality allows you to save independent iterations (e.g., `circuit_v1.json`, `circuit_v2_unified.json`) locally and pick up right where you left off.

---

## 🕹️ User Manual / Manual de Usuario

### 🇬🇧 English: How to Use the Tool

#### 1. Managing Circuits
- **Create a Circuit:** In the panel sidebar, look for **"1. SELECCIONAR CIRCUITO"**. Enter a circuit number (e.g., `1`) and a descriptive name (e.g., `Kitchen`), then click the **`+`** button.
- **Select Active Circuit:** Use the dropdown menu to choose which circuit you want to work on. Any lights or switches you place will be automatically linked to this selection.

#### 2. Placing and Editing Elements
- **Set the Tool Mode:** Click **`💡 Luz` (Light)** or **`🎛️ Interruptor` (Switch)** to select your active tool.
- **Choose Light Subtypes:** If you select **Light**, a secondary dropdown menu will appear. Use it to toggle between *Circular Standard Light*, *Square Reflector*, *Horizontal LED Strip*, or *Vertical LED Strip*.
- **Add to Blueprint:** Click anywhere directly on the map area to drop the chosen element.
- **Move Elements (Drag & Drop):** Click and hold any node on the blueprint, drag it to its new location (e.g., aligning along a specific wall), and release.
- **Delete Elements:** To remove an element permanently, **Right-Click** on its node while *Simulation Mode is OFF*.

#### 3. Bundling Switches into Wall Boxes
- **Select Multiple Switches:** Go to section **"3. GESTIONAR CAJAS DE PARED"** on the sidebar. Hold the **`CTRL`** key (or `CMD` on Mac) and click on up to 3 individual switches from the list.
- **Assemble:** Click **`📦 Unificar Seleccionados en Caja`**. The individual squares will vanish from the blueprint, replaced by a single, sleek vertical rectangle box centered at their average location. You can drag this box as a single unit onto your wall lines.
- **Disassemble / Fix Mistakes:** If you made a mistake or want to ungroup a box, simply **Right-Click** directly on the vertical box on the blueprint. It will instantly dissolve, and all inner switches will pop right back out as individual elements.

#### 4. Live Energy Simulation
- **Activate Live Grid:** Click the main **`⚡ ACTIVAR SIMULACIÓN`** button. The editing tools will lock up to prevent accidental modifications.
- **Toggle Power Distribution:** - You can flip the power toggles (switches) directly inside the sidebar list, **OR**
  - Click directly on any light node or modular box key on the blueprint map.
- **Visual Feedback:** When a circuit goes live, all linked lamps (circles, squares, and lines) will turn bright yellow/white with glowing physics. In bundled wall boxes, only the specific horizontal strip tied to that live circuit will flip to a vibrant **green**, letting you isolate power paths visually.

#### 5. Version Control & File Management
- **Save Progress:** Click **`💾 Guardar JSON`**. It downloads an encrypted text file locally to your machine with your exact coordinates, definitions, and box modules. Name it something like `wiring_layout_v1.json`.
- **Load Progress:** Click **`📂 Cargar JSON`**, choose your previously saved file, and the blueprint map will instantly restore back to its recorded layout state.

---

### 🇪🇸 Español: Cómo usar la herramienta

#### 1. Gestión de Circuitos
- **Crear un Circuito:** En el panel lateral, dirígete a **"1. SELECCIONAR CIRCUITO"**. Ingresa un número (ej: `1`) y un nombre identificativo (ej: `Cocina`), luego presiona el botón **`+`**.
- **Seleccionar Circuito Activo:** Usá el menú desplegable para elegir en qué circuito querés trabajar. Todas las luces o llaves que coloques a partir de ese momento quedarán vinculadas a él.

#### 2. Colocación y Edición de Elementos
- **Cambiar de Herramienta:** Hacé clic en los botones **`💡 Luz`** o **`🎛️ Interruptor`** para definir qué vas a colocar.
- **Elegir Tipo de Luminaria:** Si seleccionás la herramienta de Luz, se abrirá un submenú abajo. Podés alternar entre *Luz Común Circular*, *Reflector Cuadrado*, *Tira LED Horizontal* o *Tira LED Vertical*.
- **Añadir al Plano:** Hacé clic izquierdo en cualquier parte de la imagen del plano para estampar el componente.
- **Arrastrar (Drag & Drop):** Mantené presionado el clic izquierdo sobre cualquier nodo del mapa, movelo hacia su nueva posición (siguiendo los muros o bocas originales) y soltalo.
- **Eliminar Componentes:** Para borrar de forma definitiva un elemento suelto, hacé **Click Derecho** sobre su nodo en el plano (*mientras la simulación esté apagada*).

#### 3. Agrupar Interruptores en Cajas de Pared
- **Selección Múltiple:** Ve a la sección **"3. GESTIONAR CAJAS DE PARED"** en la barra lateral. Mantené presionada la tecla **`CTRL`** de tu teclado (o `CMD` en Mac) y hacé clic sobre las llaves individuales (hasta 3) que quieras unificar desde la lista.
- **Unificar:** Presioná el botón **`📦 Unificar Seleccionados en Caja`**. Verás que los cuadrados sueltos desaparecen del plano y nace un único rectángulo fino vertical (estilo bastidor de pared real). Podés arrastrar esta caja entera sobre el muro del plano.
- **Desarmar / Corregir Errores:** Si te equivocaste de llave o querés disolver un grupo, simplemente dale **Click Derecho** directamente al bastidor vertical sobre el plano. La caja se desarmará al instante y los interruptores volverán a aparecer sueltos donde estaban originalmente.

#### 4. Simulación de Energía en Vivo
- **Encender el Tablero:** Hacé clic en el botón principal **`⚡ ACTIVAR SIMULACIÓN`**. Las herramientas de edición se bloquearán para evitar alteraciones accidentales.
- **Operar los Circuitos:** - Podés encender y apagar los interruptores térmicos desde las perillas en la lista lateral, **O**
  - Podés hacer clic izquierdo directamente sobre cualquier lámpara o módulo de tecla en el plano.
- **Lectura Visual:** Al energizar un circuito, todas las luminarias asociadas (círculos, rectángulos y líneas) cambiarán a un color amarillo/blanco brillante con un halo reflectivo. En las cajas unificadas de pared, **solo la franja horizontal correspondiente a ese circuito cambiará a verde vivo**, emulando qué tecla física está activa en el ambiente.

#### 5. Guardado de Versiones y Archivos
- **Exportar Trabajo:** Hacé clic en **`💾 Guardar JSON`**. Se descargará un archivo de datos liviano a tu computadora. Podés guardarlo con nombres secuenciales (ej: `plano_v1.json`, `pruebas_uniones_v2.json`).
- **Importar Trabajo:** Hacé clic en **`📂 Cargar JSON`**, seleccioná tu archivo guardado y el simulador reconstruirá instantáneamente todo tu progreso, coordenadas y cajas modulares sobre el plano sin perder nada.

---

## 🛠️ Technology Stack

- **Frontend:** HTML5, CSS3 (Modern Flexbox grid, CSS Variable architecture, Keyframe Animations).
- **Interactions:** Native Vanilla JavaScript DOM manipulation, multi-pointer Drag-and-Drop system, custom Context Menu event listeners.
- **Data Persistence:** Client-side JSON file encoding & parsing utilizing `FileReader` streams.

---

## 📂 Installation & Local Usage

Since the architecture is built completely on client-side environments, there are no server-side compilers or node packages required.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/santimaldonado2/electrodesign.git](https://github.com/santimaldonado2/electrodesign.git)