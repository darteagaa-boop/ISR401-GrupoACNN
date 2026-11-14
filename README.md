# ISR401-GrupoACNN

Repositorio del **grupo ACNN** para la asignatura **Ingeniería de Requerimientos (ISR-401)**,
4.º nivel, Paralelo B, Universidad Técnica Estatal de Quevedo.

Docente: Gleiston Cicerón Guerrero Ulloa, PhD.

## Integrantes

- Arteaga Alava Danela Dayana
- Chavarría Cuenca Tahiny Mel
- Naranjo Alfonzo Anthony Alexander
- Nivela Saavedra José Ricardo

## Contenido

| Carpeta | Actividad | Archivo principal |
|---|---|---|
| `FORM-PC-01/` | Comparación de modelos de proceso de requisitos en escenarios reales | `FORM-PC-01/main.tex` |
| `PE1-U1/` | Práctica experimental 1: Ingeniería de Requisitos y Proceso de Requisitos aplicados al Sistema de gestión para un restaurante con IA | `PE1-U1/main.tex` |

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

Estructura de `PE1-U1/` (integrantes: Arteaga Alava Danela Dayana, Chavarría Cuenca Tahiny Mel y Naranjo Alfonzo Anthony Alexander):

| Archivo | Contenido | Responsable |
|---|---|---|
| `main.tex` | Documento principal, une las secciones con `\input` | Danela |
| `referencias.bib` | Fuentes obligatorias [1] a [10] en estilo IEEE (`biblatex`) | Danela |
| `secciones/0-pfc.tex` | Sección 0: sistema del PFC, stakeholders y tipo de sistema | Danela |
| `secciones/2-1.tex`, `secciones/2-2.tex` | Fundamento teórico 2.1 y 2.2 | Danela |
| `secciones/2-3.tex`, `secciones/2-4.tex` | Fundamento teórico 2.3 y 2.4 | Tahiny |
| `secciones/2-5.tex`, `secciones/2-6.tex` | Fundamento teórico 2.5 y 2.6 | Anthony |
| `secciones/3-requisitos.tex` | Tabla de 15 requisitos aplicada al PFC | Tahiny |
| `secciones/3-propiedades.tex` | Evaluación de los requisitos con IEEE 29148 | Danela |
| `secciones/3-contexto.tex` | Límite del sistema, visión y ocho perspectivas de contexto | Anthony |
| `secciones/3-actores.tex` | Actores del proceso y framework de IR aplicado | Anthony |
| `secciones/3-proceso.tex` | Aplicación del proceso de requisitos | Danela |
| `secciones/3-mapa.tex` | Mapa conceptual integrador (`figuras/`) | Danela |
| `secciones/conclusiones.tex` | Cinco conclusiones | Todos |
| `secciones/anexo-a.tex`, `secciones/anexo-b.tex` | Anexos A y B | Danela |
| `secciones/declaracion-ia.tex` | Declaración de uso de IA | Todos |

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

### Compilar PE1-U1

Se usan el mismo compilador, el mismo orden de comandos y las mismas dependencias,
desde la carpeta `PE1-U1`. Además requiere los paquetes `graphicx` para las figuras y `pdflscape` para la página horizontal del mapa conceptual.

```bash
cd PE1-U1
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

El resultado es `PE1-U1/main.pdf`.
