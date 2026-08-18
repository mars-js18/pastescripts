# 🛡️ Aplicación Web Sigilosa (Stealth Notes & Corporate Facade)

Aplicación web de un solo archivo (HTML, CSS y Vanilla JavaScript) diseñada para funcionar con máximo sigilo en entornos corporativos (centros de atención a clientes, soporte, etc.), camuflando tus apuntes, guiones y notas personales tras una fachada de **Monitor de Latencia de Red Corporativo**.

---

## 🚀 Características Principales

### 1. La Fachada Corporativa (Modo Normal)
* **Apariencia Realista:** Se ve exactamente como un sistema interno de monitoreo de red (*"Global Network Diagnostic Console v4.8.2"*).
* **Gráfica de Latencia en Vivo:** Dibujada con HTML5 Canvas con fluctuaciones realistas de ping.
* **Consola de Logs:** Flujo simulado continuo de eventos de diagnóstico y red en tiempo real.
* **Seguridad Visual:** Libre de cualquier elemento sospechoso si un supervisor o compañero pasa cerca.

### 2. Disparador Secreto & Botón de Pánico
* **Palabra Secreta:** Teclea la palabra **`open123`** en cualquier momento mientras estés en la página para abrir la biblioteca oculta.
* **Atajo de Teclado:** Presiona `Ctrl + Shift + X`.
* **Disparador con Mouse:** Haz triple clic en el texto disimulado de la esquina inferior derecha (*"SysID: 0x8F92A"*).
* **🚨 BOTÓN DE PÁNICO INSTANTÁNEO:** Presiona la tecla **`Escape` (ESC)** en cualquier momento desde el modo secreto. La interfaz desaparecerá **al instante (0 ms)** y volverá a mostrar el monitor corporativo.

### 3. Biblioteca Oculta & Consumo de GitHub Gist
* **Arquitectura Dinámica:** Conéctate a un GitHub Gist (o cualquier JSON público). Solo necesitas publicar la web una vez y actualizar tus apuntes desde tu casa editando el Gist.
* **Modo Oscuro Minimalista:** Interfaz tipo IDE / Terminal oscura con tipografía monoespaciada (`Consolas`, `JetBrains Mono`, `Fira Code`).
* **Buscador en Tiempo Real:** Filtra tus apuntes e instrucciones al instante por palabras clave.

### 4. Optimizado para el Bloc de Notas (Notepad de Windows)
* **Formato `<pre>` Conservado:** Mantiene todos los saltos de línea, sangrías y listas.
* **Copia Inteligente:** Convierte automáticamente los saltos de línea al estándar de Windows (`\r\n`) para que al pegar en Notepad no se deforme ni pierda formato.

---

## 🛠️ Cómo Configurar tu GitHub Gist

### Paso 1: Crear el Gist en GitHub
1. Entra a [https://gist.github.com/](https://gist.github.com/).
2. Ponle un nombre al archivo terminando en `.json` (ejemplo: `mis_apuntes.json`).
3. Copia la estructura JSON que se muestra a continuación.
4. Haz clic en **"Create public gist"** (o Secret Gist).
5. Haz clic en el botón **"Raw"** del Gist para obtener el enlace directo.

### Paso 2: Estructura JSON para tu Gist
```json
{
  "title": "Mis Apuntes de Trabajo",
  "updatedAt": "2026-08-17",
  "categories": [
    {
      "id": "scripts-atencion",
      "name": "📞 Scripts de Atención",
      "items": [
        {
          "title": "Saludo Inicial",
          "content": "Buenas tardes, le atiende [Tu Nombre]. ¿En qué puedo ayudarle hoy?\n\n1. Validar nombre completo.\n2. Confirmar número de cuenta."
        },
        {
          "title": "Cierre de Llamada",
          "content": "Gracias por comunicarse con nosotros. Su número de reporte es #[FOLIO]. ¡Excelente día!"
        }
      ]
    },
    {
      "id": "procedimientos",
      "name": "⚙️ Procedimientos y Escalaciones",
      "items": [
        {
          "title": "Escalar a Nivel 2",
          "content": "Para escalar caso a Nivel 2:\n- Enviar correo a soporte-n2@empresa.com\n- Incluir logs de pruebas y número de serie."
        }
      ]
    }
  ]
}
```

### Paso 3: Conectar la URL a la Aplicación Web
Tienes dos formas sencillas de hacerlo:

* **Opción A (Desde el Código HTML):**
  Abre [index.html](file:///c:/Users/guill/Downloads/apps/studyW/index.html), busca la constante `DEFAULT_GIST_URL` en el bloque `<script>` (alrededor de la línea 400) y pega la URL Raw de tu Gist:
  ```javascript
  const DEFAULT_GIST_URL = "https://gist.githubusercontent.com/TU_USUARIO/HASH_GIST/raw/mis_apuntes.json";
  ```

* **Opción B (Desde la Interfaz Secreta):**
  Abre el modo secreto (`open123` o `Ctrl + Shift + X`), haz clic abajo a la izquierda en **"⚙️ Configurar URL de Gist"**, pega tu enlace Raw y presiona **Guardar y Sincronizar**. (Se guardará en el navegador).

---

## 📁 Estructura del Proyecto

* [`index.html`](file:///c:/Users/guill/Downloads/apps/studyW/index.html) - Aplicación web completa en un solo archivo autosuficiente. Contiene todo el marcado HTML, estilos CSS y lógica de JavaScript.
* `README.md` - Documentación de uso y configuración.

---

## 💡 Instrucciones de Despliegue
Al ser un único archivo `index.html` sin dependencias externas:
1. Puedes alojarlo gratis en **GitHub Pages**, **Vercel**, **Netlify** o un servidor interno.
2. O simplemente abrir el archivo `index.html` directamente en cualquier navegador de tu equipo de trabajo.
