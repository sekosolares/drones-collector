<script>
  let listOfDrones = [
    'Drone 1',
    'Heliway 901 HS'
  ]
</script>

<h3> List of Drones: </h3>

<ul>
  {#each listOfDrones as drone}
    <li>{drone}</li>
  {/each}
</ul>