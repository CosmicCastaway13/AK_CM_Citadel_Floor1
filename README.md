# AK_CM_Citadel_Floor1
Version 1

When migrated to the master file, first thing to do is add 3 variables to the player class:
  - HasRedKey
  - HasBlueKey
  - HasElevatorKey
All initialized at FALSE.

Next, open up the following 6 BP's:
  - BP_Red_Key
  - BP_Blue_Key
  - BP_Elevator_Key
  - Red_Key_Door
  - Blue_Key_Door
  - Elevator_Key_Door
Then, where the comment implies, add a cast to the player character and replace the corresponding key getter branch condition.

The dialog component can be used to simulate an elevator interaction:
  [Enters elevator and interacts with button]
    Would you like to go up?
      Yes
      or
      No
    Yes -> next floor
    No -> remain on current floor
