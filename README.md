# Introduccion

Este proyecto es puramente una practica por hobbie de como trabajar en equipo, creando un blog de programacion acerca de las materias que dan en el ITNLD, mas encima algunas explicaciones y ejemplos breves de tecnologias variadas.

## Indice
- [Como funciona astro](#como-funciona-astro)
- [Forma de trabajo](#forma-de-trabajo)
    - [GIT](#git)
        - [Ramas](#ramas)
        - [Commits](#commits)
    - [Paginas](#paginas)
        - [Frameworks](#ramas)

## Como funciona astro

Astro es un framework para sitios web conducido por el contenido, capaz de poder combinar otros frameworks, compiladores o librerias de componentes y UI, pudiendo combinar el contenido de estas en un archivo .astro.

Para mas informacion, [consulta la documentacion oficial de Astro](https://docs.astro.build/es/getting-started/).

# Forma de trabajo

## GIT

Git es la herramienta de gestion de versiones por excelencia que se utilizara para este proyecto, tratando de incorporar CI/CD para practica de DevOps, y las pull request para practica de validacion de versiones integradoras al proyecto.

### Ramas
Como este proyecto se espera tener una gran escala, mas que nada porque sera un pasatiempo mas que un trabajo formal y se puede extender incalculablemente, dependiendo de la motivacion que se tenga al actualizarlo, se trabajara por ramas.

Se recomienda que cada seccion del apartado ./src/pages/[pagina a manipular] se cree una nueva rama dentro de git para poder alterar solamente ese apartado, sin riesgo alguno de afecta el resto del trabajo y posiblemente tener que reparar cosas que ya funcionaban (Si ya jala, ni le muevas).

### Commits

Cada actualizacion, mas que nada para practicar el trabajo en equipo dentro de un "**proyecto real**", se recomienda que cada **"git add [carpeta(s)]"**, sea de forma agrupada y consisa, evitando el tipico **"git add ./"**, y asi poder hacer commits mas completos, ya sea descriptivos o breves, para facilitar la busqueda de commits antiguos si algo sale mal.

Ejemplo:

```
git add ./src/pages/css/introduction/*
git commit -m "Se actualizo el contenido de la introduccion a CSS"
git push
```

## Paginas

Las paginas, como se piensa hacer un blog estatico, no se utilizara alguna base de datos (almenos por ahora) para cargar informacion dinamica. Asi que, la forma de como se organizara la rama de carpetas sera la siguiente:

```
pages 
  | -> css
  |   | -> introduccion
  |         | -> index.astro
  | -> carpeta
  | -> carpeta2
  | -> carpeta3
    | -> archivo.astro
    | -> archivo.ext
```

### Frameworks

Existe una diversa variedad de frameworks soportados en Astro, pero actualmente se incorporaron 3 frameworks por comodidad, conocimiento o por meramente experimentar algo nuevo con lo que trabajar.

<div style="height:50px">
<img src="https://gitlab.com/uploads/-/system/group/avatar/10896369/React.png">
<img src="https://www.geekandjob.com/uploads/wiki/81d4003ffa25ea82868e1786f043d4c0.png">
<img src="https://bradlc.gallerycdn.vsassets.io/extensions/bradlc/vscode-tailwindcss/0.9.1/1666201751061/Microsoft.VisualStudio.Services.Icons.Default">
</div>

- [React](https://react.dev/learn)
- [Svelte](https://svelte.dev/docs/introduction)
- [Tailwind](https://tailwindcss.com/)

Si se desea integrar algun otro framework, por comodidad, gusto, o ganas de aprenderlo usando este blog como practica, hagan la solicitud en la [pagina de github del proyecto](https://github.com/Chenomorfo/BlogTec/pulls) como una pull request
## Proximamente...