<script>

  import { onMount } from "svelte";
  import Typed from "typed.js";
  export let profileImage;
  export let projects;
  export let skills;
  onMount(() => {
    var typed = new Typed(".multi-text", {
      strings: [" a coder", " a developer"],
      typeSpeed: 130,
      backSpeed: 130,
      loop: true
    });
  });
</script>


<style>
  /*.cols {*/
  /*  border-radius: 2%;*/
  /*  margin-bottom: 5%;*/
  /*  width: 100%;*/
  /*  height: 90%;*/
  /*  z-index: 1;*/
  /*  background-color: white;*/
  /*  position: relative;*/
  /*}*/

  .image-hello {
    display: flex;
    height: 9%;
    width: 100%;
    flex-direction: row;
    position: relative;
  }

  .profile-image-container {
    position: absolute;
    aspect-ratio: 1;
    height: 250%;
    border-radius: 50%;
    right: 50%;
    box-shadow: 5px 5px 2px rgba(0, 0, 0, 0.4);
    background-color: black;
    display: inline-block;
    top: -150%;
  }

  .profile-image {
    height: 100%;
    border-radius: 50%;
  }

  .multi-text-header {
    margin-left: 35%;
  }

  h1 {
    display: block;
    font-size: 1em;
    font-weight: 900;
    color: black;
    font-family: "Calibri Light";
  }

  .multi-text {
    color: grey;
    font-size: 1.5em;
  }

  .projects {
    margin-left: 10px;
    font-family: Arial;
    font-size: 30px;
    color: black;
  }

  .experience {
    display: flex;
    flex-direction: column;
    border-top-style: solid;
    border-left-style: solid;
    border-right-style: solid;
    border-color: grey;
    border-radius: 10px;
    border-width: 2px;
    width: 90%;
    box-shadow: 2px -4px 2px rgba(0, 0, 0, 0.4);
    align-items: start;
    justify-content: space-around;
    z-index: 150;
  }

  .experience li {
    color:  black;
    margin-bottom: 1px;
    font-size: 20px;
    font-family: Arial;
    list-style: disc;
  }
  .col0{


    border-radius: 2%;
    margin-bottom: 7%;
    width: 100%;

    height: 87%;
    z-index: 1;
    background-color: white;
    position:relative;
  }
</style>

<div class="cols col0">
  <div class="image-hello">
    <div class="profile-image-container">
      <img src="{profileImage}" class="profile-image">
    </div>
  </div>

  <h1 class="multi-text-header">I'm <span class="multi-text"></span></h1>
  <h2 class="projects">PROJECTS</h2>
  <ul class="experience">
    {#each projects as project}
      <li>{project}</li>
    {/each}
  </ul>

  <h3 class="projects">SKILLS</h3>
  <ul class="experience">
    {#each skills as skill}
      <li>{skill}</li>
    {/each}
  </ul>
</div>
