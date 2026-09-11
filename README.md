# Organizador de comisiones

Aplicación web estática para encontrar alternativas de cursado sin cruces horarios a partir de un archivo Excel.

## Uso local

1. Abrí la carpeta del proyecto en VS Code.
2. Levantá un servidor local:

   ```bash
   python3 -m http.server 8000
   ```

3. Abrí `http://localhost:8000`.
4. Cargá un archivo `.xlsx` o `.xls` con la primera hoja y estas columnas:

   `elemento_nombre`, `elemento_codigo`, `comision`, `comision_nombre`, `dia_semana`, `hora_inicio`, `hora_fin`

El archivo se procesa en el navegador y no se envía a ningún servidor.

## Publicar con GitHub Pages

1. Creá un repositorio en GitHub.
2. Subí `index.html`, `README.md` y `.gitignore`.
3. En GitHub, abrí **Settings > Pages**.
4. Elegí **Deploy from a branch**, seleccioná `main` y la carpeta `/ (root)`.
5. Guardá y esperá a que GitHub genere la URL pública.

La aplicación usa Tailwind CSS y SheetJS desde CDN, por lo que necesita conexión a internet al abrirse.
