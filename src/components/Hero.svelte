<script>
  import { onMount } from "svelte"
  import { fade, fly } from "svelte/transition"
  import { cubicInOut } from "svelte/easing"

  import Greeting from "./Greeting.svelte"
  import Links from "./Links.svelte"
  import Areas from "./Areas.svelte"

  let ready = false

  function setVh() {
    const vh = window.innerHeight * 0.01
    document.documentElement.style.setProperty("--vh", `${vh}px`)
  }

  onMount(() => {
    setVh()
    window.addEventListener("resize", setVh)
    ready = true
  })
</script>

<main class="font-sans text-white bg-zinc-900">
  <div class="fill-viewport-height flex items-center justify-center">
    {#if ready}
      <div
        transition:fade={{ duration: 1000, easing: cubicInOut }}
        class="w-full text-center py-8"
      >
        <div transition:fly={{ y: 200, duration: 1000 }}>
          <Greeting />
          <Areas />
          <Links />
        </div>
      </div>
    {/if}
  </div>
</main>
