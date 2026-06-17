# Generador de Horarios — UNAB

Aplicación web de un solo archivo (`index.html`) para armar horarios sin topes a partir
de un export de detalle de docentes por NRC y la malla curricular. Corre 100% en el
navegador: no necesita servidor, base de datos ni instalación.

## Uso

1. Abre la aplicación (o el archivo `index.html` con doble clic).
2. Carga el **archivo de datos** (`Detalle_Docentes_por_NRC.xlsx`).
3. Carga la **malla curricular** (`.xlsx`) para habilitar el filtro por semestre.
4. Elige **programa** y **semestre** y pulsa **Generar horarios**.
5. Revisa el **horario completo** y los **horarios de alumno** sin topes.
6. Descarga el **Excel** con colores por curso y la glosa de asignaturas.

## Características

- Carga de archivos por arrastrar y soltar.
- Filtro por programa y por semestre (según la malla).
- Horario completo del semestre y combinaciones de alumno sin topes.
- Colores consistentes por curso, leyenda y buscador (curso, profesor, sala, NRC).
- Exportación a Excel multi-hoja con colores y glosa de asignaturas.
- Funciona offline: las librerías (SheetJS y ExcelJS) van incrustadas en el archivo.

## Tecnología

HTML + JavaScript. [SheetJS](https://sheetjs.com) para leer `.xlsx` y
[ExcelJS](https://github.com/exceljs/exceljs) para exportar con formato.
