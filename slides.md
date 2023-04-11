---
theme: seriph
titleTemplate: '%s - testsCase'
# enable presenter mode, can be boolean, 'dev' or 'build'
presenter: true
download: true
# enable slide recording, can be boolean, 'dev' or 'build'
record: 'build'
exportFilename: testsCase-exported
export:
  format: pdf
  timeout: 30000
  dark: false
  withClicks: false
  withToc: false
background: https://source.unsplash.com/collection/298137/1920x1080
class: text-center
highlighter: shiki
lineNumbers: true
info: |
  ## Team's Shopopop
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
drawings:
  persist: false
fonts:
  sans: Robot
  serif: Robot Slab
  mono: Fira Code
title: Welcome to team's Shopopop
---

# Welcome to team's Shopopop

Presentation slides for developers

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://www.shopopop.com" target="_blank" alt="Shopopop"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:debug />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
layout: cover
class: text-center
---

# Tests

```ts
expect(function).toBe(null)
```

<img src="https://nodejs.dev/static/images/brand/logos-js-right/light.svg" class="m-auto" />

---
layout: center
---

# Les tests de composant pourrait être ton meilleur arrangement

✅ À faire: Chaque test unitaire couvre une petite portion de l'application et il est coûteux de couvrir l'ensemble, alors que les tests end-to-end couvrent facilement une grande partie mais sont lent, pourquoi ne pas appliquer une approche intermédiaire et écrire des tests qui sont plus gros que les tests unitaires mais plus petits que les tests end-to-end ? Les tests de composant (Component testing) sont méconnus du monde de test mais ils offrent le meilleur des deux mondes: des performances raisonnable et la possibilité d'appliquer le pattern TDD + une couverture correcte et réaliste

Les tests de composant se concentrent sur "l'unité" du microservice, ils fonctionnent sur l'API, ne mock rien qui appartient au microservice lui-même (une vrai DB, ou au moins une version in-memory de cette DB) mais stub tout ce qui est externe, comme les appels à d'autres microservices. En faisant ça, on test ce que l'on déploie, on approche l'application de l'extérieur vers l'intérieur et on gagne en confiance dans un laps de temps raisonnable.

---
layout: center
class: text-center
---

# Thank's

<img src="https://user-images.githubusercontent.com/94382341/159370370-cb8a63c8-2a42-413c-a659-2ce5662eecbf.png" class="m-30 h-30" />

[GitHub](https://github.com/stephen-shopopop)
