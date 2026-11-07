# ISR401-GrupoACNN

Repositorio del **grupo ACNN** para la asignatura **Ingeniería de Requerimientos (ISR-401)**,
4.º nivel, Paralelo B, Universidad Técnica Estatal de Quevedo.

Docente: Gleiston Cicerón Guerrero Ulloa, PhD.

## Integrantes

- Arteaga Alava Danela Dayana (líder)
- Chavarría Cuenca Tahiny Mel
- Naranjo Alfonzo Anthony Alexander
- Nivela Saavedra José Ricardo

## Contenido

| Carpeta | Actividad | Archivo principal |
|---|---|---|
| `FORM-PC-01/` | Comparación de modelos de proceso de requisitos en escenarios reales | `FORM-PC-01/main.tex` |

Estructura de `FORM-PC-01/`:

| Archivo | Contenido | Responsable |
|---|---|---|
| `main.tex` | Documento principal, une las secciones con `\input` | Danela |
| `referencias.bib` | Referencias en estilo IEEE (`biblatex`) | Danela |
| `secciones/criterios.tex` | Criterios de comparación | Danela |
| `secciones/modelo-cascada.tex` | Modelo en cascada | Tahiny |
| `secciones/modelo-iterativo.tex` | Modelo iterativo | Anthony |
| `secciones/modelo-agil.tex` | Modelo ágil | José |
| `secciones/escenario-gad.tex` | Escenario: sistema de un GAD con contrato público | Danela |
| `secciones/escenario-embebido.tex` | Escenario: sistema embebido de una planta | Tahiny |
| `secciones/escenario-app.tex` | Escenario: aplicación móvil de un emprendimiento | Anthony |
| `secciones/escenario-cooperativa.tex` | Escenario: plataforma de una cooperativa | José |
| `secciones/matriz.tex` | Matriz escenario por modelo (cada integrante llena su fila) | Todos |
| `secciones/framework-pohl.tex` | Framework de Pohl aplicado al GAD | Danela |

## Cómo compilar

### Compilador y orden de comandos

Compilador: `pdflatex`, con `biber` para la bibliografía. Desde la raíz del repositorio:

```bash
cd FORM-PC-01
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

El resultado es `FORM-PC-01/main.pdf`.

### Dependencias

- Distribución LaTeX: TeX Live 2022 o posterior, o MiKTeX actualizado.
- Clase: `IEEEtran`.
- Paquetes: `fontenc`, `inputenc`, `babel` (idioma `spanish`), `lmodern`,
  `microtype`, `csquotes`, `amsmath`, `amssymb`, `booktabs`, `float`,
  `tabularx`, `array`, `longtable`, `url`, `hyperref` y `biblatex`
  con el estilo `ieee` (paquete `biblatex-ieee`).
- Gestor de bibliografía: `biber`.

En Overleaf: subir la carpeta `FORM-PC-01` completa, elegir el compilador
pdfLaTeX y compilar. Overleaf ejecuta `biber` automáticamente.
