<script>
  let title = "il Pomodoro";
  import TaskList from './TaskList.svelte';
  import PomodoroTimer from './PomodoroTimer.svelte';
</script>

<main>
  <h1>{title}</h1>
  <PomodoroTimer/>
  <TaskList/>
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: var(--accent);
    text-transform: uppercase;
    font-size: 6em;
    margin: 0;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
