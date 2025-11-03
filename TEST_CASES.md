# Test Case – ISSUE-1: Using MainMenu system on the platform
**Related issue:** #1 
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and is on the MainMenu

## Steps (Given–When–Then)
1. **Given** MainMenu is open
2. **When** Press "Start"
3. **Then** Gamen starts

## Expected Results
- Litle to no delay in start

## Notes
- **Aditional Notes:** Other buttons are not yet implementet



# Test Case – ISSUE-2: Game pause when playing
**Related issue:** #2 
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and not in menu

## Steps (Given–When–Then)
1. **Given** Game is runnig
2. **When** Pause key is pressed
3. **Then** Game animations and logic pauses. PausMenu appears

## Expected Results
- Game stops until unpaused

## Notes
- **Aditional Notes:** Game runs again when return or the pause button is selected



# Test Case – ISSUE-3: Game pause restrictions
**Related issue:** #3 
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and is on any Menu

## Steps (Given–When–Then)
1. **Given** Game is in a Menu state
2. **When** Pause key is pressed
3. **Then** Pause menu should not appear

## Expected Results
- Nothing should happend

## Notes
- **Aditional Notes:**



# Test Case – ISSUE-4: Does UI elements scale correctly on screen
**Related issue:** #4 
**Type:** Functional Test

## Preconditions
- Scenario: Game is running

## Steps (Given–When–Then)
1. **Given** UI is wissible
2. **When** Scale screensize
3. **Then** UI stays contained on screen

## Expected Results
- User can see the whole UI

## Notes
- **Aditional Notes:** Chek all diferend UI menues (Main-, Pause-, Pssiveupgrade-menues)



# Test Case – ISSUE-5: Movement
**Related issue:** #5 
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and not in menu

## Steps (Given–When–Then)
1. **Given** Game is not paused
2. **When** User moves character by WASD (on keyboard) or joystick (on mobile)
3. **Then** Character moves to directed way

## Expected Results
- Character moves as expected

## Notes
- **Aditional Notes:** boundaries = Character can not leave the arena.



# Test Case – ISSUE-6: Can player leave the arena
**Related issue:** #6
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and not in menu

## Steps (Given–When–Then)
1. **Given** Game is not paused and playloop is on
2. **When** Character tryes to leaf the arena
3. **Then** Bounderies push back.

## Expected Results
- Character is unable to escape the arena and is pushed back stronger the further they try to push into the edge

## Notes
- **Aditional Notes:** Push feels like air/wind pushing on the player




# Test Case – ISSUE-7: Killing enemies
**Related issue:** #7
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and not in menu

## Steps (Given–When–Then)
1. **Given** Game is not paused and playloop is on
2. **When** The player attacks enemy characters with the weapons provided
3. **Then** Enemy character is destroyed and drops an xp item

## Expected Results
- Enemy character is destroyed

## Notes
- **Aditional Notes:** Killing an enemy character may require multiple hits



# Test Case – ISSUE-8: Does enemy characters stack on each other
**Related issue:** #8
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and not in menu

## Steps (Given–When–Then)
1. **Given** Game is not paused
2. **When** Several enemy characters appear on the field.
3. **Then** Enemy characters follow the player and if the player moves around the circle, the characters' movement places them in a smaller circle.

## Expected Results
- Enemy characters cannot stack.

## Notes
- **Aditional Notes:** Enemy characters have slow and low thrust relative to each other.



# Test Case – ISSUE-9: Enemy movement (Dasher enemy “GrassHopper”)
**Related issue:** #9
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and not in menu

## Steps (Given–When–Then)
1. **Given** Game is not paused and Grasshopper enemy is present
2. **When** When a Grasshopper enemy gets close enough to the player
3. **Then** It will perform a dash/charge attack.

## Expected Results
- The Grasshopper enemy will make a dash/charge attack and stay in place for a moment afterwards.

## Notes
- **Aditional Notes:** The Grasshopper enemy also has a separate animation before attacking "charging the attack"



# Test Case – ISSUE-10: Collecting Xp
**Related issue:** #10
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and not in menu

## Steps (Given–When–Then)
1. **Given** Game is not paused
2. **When** When a player kills an enemy, they drop an XP orb.
3. **Then** The player can collect XP by moving close enough to an orb for it to automatically accumulate.

## Expected Results
- The XP orb moves towards the player and the player's XP number on the screen increases.

## Notes
- **Aditional Notes:** The XP orb has its own animation where it moves smoothly towards the player when the player is close enough to collect XP.

# Test Case – ISSUE-11: Passive upgrades when offered
**Related issue:** #11
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and not in menu

## Steps (Given–When–Then)
1. **Given** Game is not paused.
2. **When** When the player collects XP and reaches the next level.
3. **Then** An update window will automatically start.

## Expected Results
- When a new level is reached, the game stops and the player is offered three different upgrade packages.

## Notes
- **Aditional Notes:** The player can track the progress of reaching the required amount of Xp for the next level in the Xp view in the upper right corner. Reaching the next level may require more than one Xp orb.



# Test Case – ISSUE-12: Weapon upgrades when offered
**Related issue:** #12
**Type:** Functional Test

## Preconditions
- Scenario: Game is running and not in menu

## Steps (Given–When–Then)
1. **Given** Game is not paused
2. **When** Elite enemy killed.
3. **Then** The weapon upgrade or new weapon selection menu will launch.

## Expected Results
- The player can choose a weapon upgrade or a new weapon from the menu.

## Notes
- **Aditional Notes:** Requires elite enemy killing