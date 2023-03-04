<script>
  let listOfDrones = [
    'Drone 1',
    'Heliway 901 HS'
  ]
  function addDrone() {
    const newDroneName = document.getElementById("NewDrone");
    listOfDrones = [...listOfDrones, newDroneName.value];
    newDroneName.value = '';
  }
</script>

<a href="/"> Home </a>

<h3> List of Drones: </h3>


<input type="text" name="newDrone" id="NewDrone">
<button on:click={addDrone}>Add Drone</button>
<ul>
  {#each listOfDrones as drone}
    <li>{drone}</li>
  {/each}
</ul>