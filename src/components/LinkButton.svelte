<script>
  export let href = "#"
  export let icon = ""
</script>

<a
  {href}
  class="flex mx-8 xs:mx-0 justify-center items-center gap-2 transition ease-in-out border-2 px-4 py-2 rounded border-gray-700 text-slate-400 hover:bg-gray-800 "
>
  {#if icon}<span>{icon}</span>{/if}
  <slot />
</a>
