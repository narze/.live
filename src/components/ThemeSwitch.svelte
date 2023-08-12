<script lang="ts">
  let theme = localStorage.getItem("theme") ?? "light"

  $: {
    if (theme === "dark") {
      document.documentElement.classList.add("dark")
    } else {
      document.documentElement.classList.remove("dark")
    }

    localStorage.setItem("theme", theme)
  }

  function toggleTheme() {
    theme = theme === "light" ? "dark" : "light"
  }
</script>

<button
  on:click={toggleTheme}
  class="w-8 h-8 hover:bg-zinc-200 dark:hover:bg-zinc-800 rounded-full"
  >{theme === "light" ? "🌞" : "🌙"}</button
>
