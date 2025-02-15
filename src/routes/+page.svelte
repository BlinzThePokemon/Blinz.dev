<script>
    import Projects from './Components/projects.svelte'
    import Footer from './Components/footer.svelte'
</script>

<div class="header text-6xl font-semibold flex justify-center mt-20 color-effect"><p class="greeting">Hello Person! I'm Blinz</p></div>

<div class="flex items-center justify-center bg-gray-100 mt-5">
    <div class="w-3/5 p-6 bg-white rounded-lg shadow-lg">
      <h1 class="text-2xl font-semibold mb-4">Who Is I?</h1>
      I am Blinz. I am a beginner programmer, I began learning coding stuff about 4 years ago, starting with Scratch then to Web Dev.
      Now I am mostly focusing on Game Dev, my "dream job" is to become a Game Developer.
      <br>
      I LOVE programming.
    </div>
  </div>
  
<Projects />
<div class="flex items-center justify-center bg-gray-100 mt-5 mb-7">
    <div class="w-3/5 p-6 bg-white rounded-lg shadow-lg">
      <h1 class="text-2xl font-semibold mb-4">More About Me</h1>
      <p class="text-xl font-semibold">I Love Programming!</p>
      <p><li>I am in love with programming but am not very good at it.</li> <li>I am currently learning Svelte along with SvelteKit. I am also learning to make games in Godot</li> </p>
      <p class="text-xl font-semibold mt-2">I Also Like Games</p>
      <p><li>I have some games like - Geometry Dash, BTD 6, Trackmania, Melatonin just to name a few</li> <li>Most of the games I own have been bought by my friend <b>Jazza</b> (Who is financially an idiot), check them out <a target="_blank" href="https://jazza.dev">Here</a></li></p>
      <p class="text-xl font-semibold mt-2">I Am Addicted To Food</p>
      <p>
        <li>I am so, so addicted to food, I mean we all have a lifetime addiction of eating</li>
        <li>Anything thing sweet, I eat!</li>
        <li>I am on a sea food diet. I see food; I eat food</li>
        <li>I am also of making weird but tasty combos</li>
        <li>If its a fast-food dish just make it spicy and I will eat it!</li>
      </p>
      <p class="text-xl font-semibold mt-2">More Things I Like</p>
      <p>
        <li>Movies</li>
        <li>Not too much, but reading like Geronimo Stilton</li>
      </p>
      <p class="text-xl font-semibold mt-2">Tech</p>
      <p>
        <li>I am learning Svelte, and Sveltekit. Hail Lord Matia</li>
        <li>I am also making games in Godot</li>
      </p>
    </div>
  </div>
  
<Footer />

<style>
::selection {
    background: orange;
}
:global(body) {
    font-family: 'Poppins', sans-serif;
  }
  a{
        text-decoration: underline;
        transition: all 200ms;
        text-decoration-thickness: 2px;
    
    &:hover{
        font-size: larger;
    }
    }
</style>