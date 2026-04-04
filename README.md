# Proyectos LaTeX
Repositorio para la gestión de documentos en LaTeX (prácticas, presentaciones y textos académicos).

## Estructura
.
├── ejercicios/ # Ejercicios y documentos principales
│ ├── out_aux/ # Archivos auxiliares de compilación (ignorados en github, se crearán automáticamente al compilar)
│ ├── out_pdf/ # PDFs generados (ignorados)
│ └── *.tex # Archivos fuente
├── Presentaciones_curso_BD/
    ...
├── Textos_tesis/
    ...
└── .vscode/ # Configuración de VS Code


## Requisitos

- LaTeX (recomendado: TeX Live o MiKTeX)
- `latexmk` (para compilación automática)
- Editor recomendado: VS Code + extensión LaTeX Workshop

## Compilación

Desde la carpeta del archivo `.tex`:

```bash
latexmk -pdf -output-directory=out_pdf -aux-directory=out_aux archivo.tex