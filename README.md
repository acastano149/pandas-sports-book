# Instrucciones de Compilación y Uso
## 0. Inicializar el Libro
https://acastano149.github.io/pandas-sports-book/

## 1. Renderizar el Libro (Estático)

Para generar la web "normal" (HTML estático), abre una terminal en esta carpeta (`pandas_for_tidyverse_sports`) y ejecuta:

```bash
quarto render
```

Esto generará una carpeta `_book/` con el HTML. Puedes abrir `_book/index.html` en tu navegador.

## 2. Modo Interactivo (Live Code) - Experimental

¿Quieres que los usuarios puedan **ejecutar y editar** el código Python directamente en el navegador (sin instalar Python)?

Necesitas la extensión **Quarto Live** (basada en Pyodide/WASM).

### Paso A: Instalar la extensión
Ejecuta esto en tu terminal (te pedirá confirmación, di "Yes"):

```bash
quarto add r-wasm/quarto-live
```

### Paso B: Configurar
Avísame si has instalado la extensión y yo puedo:
1. Modificar `_quarto.yml` para activar el filtro `live`.
2. Convertir los bloques de código de `{python}` a `{pyodide-python}`.
3. Añadir ejercicios interactivos con feedback.

Esto permitirá que tu estudiante de doctorado practique directamente en la web que le envíes, ¡incluso desde el móvil!
