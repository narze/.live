<script>
  import LinkButton from "./LinkButton.svelte"
  import CodeIcon from "./CodeIcon.svelte"
  import YoutubeIcon from "./YoutubeIcon.svelte"
  import NoteIcon from "./NoteIcon.svelte"
  import ChatIcon from "./ChatIcon.svelte"
  import BriefcaseIcon from "./BriefcaseIcon.svelte"
  import TwitchIcon from "./TwitchIcon.svelte"
  import HacktoberFestIcon from "./HacktoberFestIcon.svelte"
</script>

<div class="flex flex-col gap-4">
  <div class="flex flex-col xs:flex-row flex-wrap gap-4 justify-center mt-8">
    <LinkButton href="https://10k.narze.live">💸 10k Planner (New!)</LinkButton>
    <LinkButton href="https://garden.narze.live"><NoteIcon />Garden</LinkButton>
    <LinkButton href="https://chat.narze.live"><ChatIcon />ChatOS</LinkButton>
  </div>

  <div class="flex flex-col xs:flex-row flex-wrap gap-4 justify-center">
    <LinkButton href="https://github.com/narze"><CodeIcon />GitHub</LinkButton>
    <LinkButton href="https://youtube.narze.live"
      ><YoutubeIcon />YouTube</LinkButton
    >
    <LinkButton href="https://twitch.narze.live"
      ><TwitchIcon />Twitch</LinkButton
    >
    <LinkButton href="https://resume.narze.live"
      ><BriefcaseIcon />Résumé</LinkButton
    >
  </div>
</div>
