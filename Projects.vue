<template>
  <section>
    <h1>Projects</h1>
    <p>A few things I've built while learning </p>
    <!--
    -<ul>: unordered list = bulleted list
    -<ol>: ordered list = numbered list
    -<li>: list item. 
    -->
      <ul>
        <li
          v-for="project in Projects"
          :key="project.id"
          class="project-item"

        >
        <div>{{ project.name }}</div>
        <div>{{ project.desc }}</div>
        <div>{{ project.tag }}</div>
        <!-- Span is an inline element-->
      
      </li>

      </ul>

  </section>
</template>

<script setup>
let Projects=[
  { id: 1,
    name: "lorem",
    desc: "desc",
    tag: " Vue 3"
  },
    { id: 2,
    name: "lorem",
    desc: "desc",
    tag: " Vue 3"
  },
    { id: 3,
    name: "lorem",
    desc: "desc",
    tag: " Vue 3"
  }
  
]

</script>

<style>
.project-list {
  list-style: none;
  display: flex;
  gap: 1rem;
  max-width: 560px;
}
.project-item{
    background-color: moccasin ;
    border: 1px solid;
    border-radius: 8px;
    gap: 500rem;
}

</style>