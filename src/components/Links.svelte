<script>
  import LinkButton from "./LinkButton.svelte"
  import CodeIcon from "./CodeIcon.svelte"
  import YoutubeIcon from "./YoutubeIcon.svelte"
  import NoteIcon from "./NoteIcon.svelte"
  import BriefcaseIcon from "./BriefcaseIcon.svelte"
</script>

<div class="flex flex-col gap-4 justify-center mt-8">
  <LinkButton href="https://garden.narze.live"><NoteIcon />Garden</LinkButton>
  <LinkButton href="https://github.com/narze"><CodeIcon />GitHub</LinkButton>
  <LinkButton href="https://www.youtube.com/c/narzelive"
    ><YoutubeIcon />YouTube</LinkButton
  >
  <LinkButton href="https://resume.narze.live"
    ><BriefcaseIcon />Résumé</LinkButton
  >
</div>

<style>
  @media (min-width: 480px) {
    .flex {
      @apply flex-row;
    }
  }
</style>
