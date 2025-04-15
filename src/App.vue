<template>
  <div>
    <BaseLayout>
      <template #logo>
        <h2>Logo</h2>
      </template>

      <template #menu-nav>
        <nav class="menu-nav">
          <ul>
            <li>Home</li>
            <li>About</li>
            <li>Contact</li>
          </ul>
        </nav>
      </template>

      <template #main>
        <h2>Main Content</h2>
        <p>This is the main content area.</p>
      </template>

      <template #aside>
        <nav class="menu-lateral">
          <ul>
            <li>Home</li>
            <li>About</li>
            <li>Contact</li>
          </ul>
        </nav>
      </template>

      <template #footer>
        <p>&copy; 2025 Programacion web dinámica</p>
      </template>
    </BaseLayout>

  </div>
</template>

<script setup lang="ts">
import BaseLayout from './layouts/BaseLayout.vue';


</script>

<style scoped>
.menu-lateral {
  display: flex;
  justify-content: center;
  align-items: center;

  ul {
    list-style: none;
    padding: 0.5em;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    li {
      width: 100%;
      margin: 0.5em 1em;
      background-color: #c45151;
      color: rgb(245, 163, 163);
      transition: 0.5s ease-in-out all;


      &:hover {
        background-color: #c4c4c4;
        color: #000;
        cursor: pointer;

      }
    }



  }
}

.menu-nav ul {
  display: flex;
  justify-content: center;
  list-style: none;

  li {
    margin: 0 1em;
    color: #fff;
    transition: 0.5s ease-in-out all;

    &:hover {
      color: #c4c4c4;
      cursor: pointer;
    }
  }

}
</style>