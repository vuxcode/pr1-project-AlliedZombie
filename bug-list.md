# Bug List

1. **Problem:** Wasted alot of time because forgot about array placement. Wrote [1] because I wanted the first one but realized a while later after building the playerDamageBy*** function that that was indeed wrong...didnt want to hardcode it into the function so thats why I really wanted the array to work 
<br> **Solution:** Should have been [0]

2. **Problem:** Coudnt get the enemy to spawn in corectly. The enemy transformed from one position to another and then in the end of the loop go back to the original point instead of continuing.
<br> 
**Solution:** change a line in css to *"animation-fill-mode: forwards"*.

3. **Problem:** The enemy would not properly randomize. The enemy was random but they could repeat after each other.
<br> **Solution:** Make a input into the function that looks for a *"PreviousEnemy"* and compare with a random enemy. The first time the function is called its *"= undefined"*

4. **Problem:** The enemy could appear more than once. So if someone spammed the buttons multiple enemies could appear because the fucntion had a timer with 500ms.
<br>**Solution:** Make a bool value that becomes true as soon as the user attacks the enemy. If this bool is true the user wont be able to attack the enemy. This bool resets as soon as a new enemy appear.