# Proyectos LaTeX
Repositorio para la gestión de documentos en LaTeX (prácticas, presentaciones y textos académicos).

## Estructura
.
├── ejercicios/ # Ejercicios y documentos principales
│ ├── out_aux/ # Archivos auxiliares (ignorado)
│ ├── out_pdf/ # PDFs generados (ignorado)
│ └── *.tex # Archivos fuente
│
├── Presentaciones_curso_BD/ # Presentaciones
│ ├── out_aux/
│ ├── out_pdf/
│ └── *.tex
│
├── Textos_tesis/ # Documentos de tesis
│ ├── out_aux/
│ ├── out_pdf/
│ └── *.tex
│
└── .vscode/ # Configuración de VS Code


## Requisitos

- LaTeX (recomendado: TeX Live o MiKTeX)
- `latexmk` (para compilación automática)
- Editor recomendado: VS Code + extensión LaTeX Workshop

## Compilación

Desde la carpeta del archivo `.tex`:

```bash
latexmk -pdf -output-directory=out_pdf -aux-directory=out_aux archivo.tex