# Muestra académica ANPADEH · Licenciatura en Urbanismo

Sitio estático para presentar trabajos académicos por etapa formativa, asignatura y nivel de evaluación.

## Contenido

- `index.html`: interfaz navegable.
- `data.js`: etapas, objetivos oficiales de asignaturas y espacios de proyectos.
- Las cuatro etapas del Plan de Estudios 2018: Inicial, Básica, Formativa e Integración Profesional.
- Catálogo de programas disponible en el Tomo II, incluyendo oferta optativa.

## Incorporar trabajos

En `data.js`, cada asignatura tiene un objeto `projects` con las categorías `alto`, `medio` y `bajo`. Añade cada proyecto como objeto con `title`, `description`, `image` (ruta dentro del repositorio), `semester` y, si corresponde, `team`. Guarda las imágenes en `assets/`.

Ejemplo:

```js
projects: {
  alto: [{ title: "Nombre del proyecto", description: "Síntesis", image: "./assets/proyecto.jpg", semester: "6.º", team: "Equipo" }],
  medio: [],
  bajo: []
}
```

Los niveles son categorías curatoriales para esta muestra. No se presentan como una escala oficial de ANPADEH.

## Publicar como GitHub Pages

En GitHub, abre **Settings → Pages**, selecciona **Deploy from a branch**, elige `main` y la carpeta `/(root)`. El sitio quedará disponible en la URL de Pages que GitHub indique.

## Fuentes

- Tomo I: estructura, etapas y organización del Plan de Estudios.
- Tomo II: programas y objetivos de asignatura.

Los documentos fuente no se copian al repositorio; se enlazan desde el catálogo.
