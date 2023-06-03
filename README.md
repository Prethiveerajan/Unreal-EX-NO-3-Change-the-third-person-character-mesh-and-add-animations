# Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations
								

## EXP:03 Change the third person character mesh and add animations
## AIM:
To Change the third person character mesh and add animations 

## PROCEDURE:

1.	Import the animation assets: Obtain the animation files for jump, walk, and idle in a compatible format such as FBX or BVH. To import the animations, go to the Content Browser panel in Unreal Engine, right-click in the desired folder, and select Import
2.	Create a Separate folder  and Import the Animations to avoid any chaos
3.	Create an animation blueprint: In Unreal Engine, animation blueprints are used to control character animations. To create a new animation blueprint, follow these steps: 
a. Right-click in the folder where you imported the mesh and select Create > Animation > Animation Blueprint. 
b. In the Animation Blueprint Editor, click on the Event Graph tab. 
c. Drag the new character mesh from the Content Browser and drop it onto the graph. 
d. Connect the Output Pose pin of the mesh node to the Final Animation Pose pin of the Final Animation Pose node.
 e. Save the animation blueprint.
4.	Open the animation blueprint: Open the animation blueprint you created for your character in the Animation Blueprint Editor.
5.	Create animation slots: Animation slots help organize different animations and control their blending. To create animation slots, follow these steps:
 a. In the AnimGraph tab of the Animation Blueprint Editor, right-click in the graph and select Add State Machine > Animation Layer. 
b. Double-click the newly created animation layer to open it.
 c. Right-click in the graph of the animation layer and select Add State Machine. 
d. Double-click the newly created state machine to open it. 
e. Right-click in the graph of the state machine and select Add State. 
f. Rename the state to "Jump" and repeat steps e and f to create states for "Walk" and "Idle".
6.	Add animation assets to states: In each state, you will assign the corresponding animation assets. To add animation assets to the states, follow these steps: a. Double-click the "Jump" state to open it. b. Right-click in the graph and select Add State Result. c. Drag and drop the jump animation asset onto the graph. d. Connect the Result node to the jump animation asset. e. Repeat steps a to d for the "Walk" and "Idle" states, assigning the appropriate animation assets.
7.	Create  required Variables for the state’s like “ISJUMP”,  “SPEED”.
8.	Set up transition rules: Transition rules determine when the character transitions between different animations. To set up transition rules, follow these steps: a. Double-click the "Jump" state to open it. b. Right-click in the graph and select Add Transition Rule. c. Drag the transition rule from the "Jump" state to the "Idle" state. d. Repeat steps a to c for the "Walk" state, creating transitions from "Idle" to "Walk" and from "Walk" to "Idle". e. Configure the transition rules based on your desired conditions. For example, you might want to trigger the transition from "Idle" to "Jump" when the character jumps, and from "Jump" to "Idle" when the jump animation is finished.
9.	Create a Anim Montage in Animation Folder To Manage the montages of the animations
10.	Connect the animation blueprint to the character blueprint: To connect the animation blueprint to the character blueprint and enable the animations in the game, follow these steps: a. Open the character blueprint associated with the third person character. b. In the Viewport tab of the Blueprint Editor, select the mesh component of the character. c. In the Details panel, under the Animation category, find the Animation Blueprint property. d. Click on the dropdown menu and select the animation blueprint you created.
11.	Test the character: Compile and save all the changes in the blueprints and animations. Now, you can test the character's jump, walk, and idle animations by clicking the Play button in the Unreal Editor.


## OUTPUT:
## MYCHAR:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/c24f083e-3ddb-47d8-849e-8f31f26bb14f)

 Prethi<ee
## ANIMATIONS:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/ecbb0553-0a1c-40d5-bbc6-46b8607a72d6)

           

            
 
## STATE MACHINE:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/995716b8-6b56-475d-bbdd-f163b0de25c3)
 
            
 
## STATE DIAGRAM:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/f857c1b6-7bfe-47ff-9ef0-83d6f3f7b9e0)

          
 
## VARIABLES:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/97a4f210-81c6-4ec2-b2e6-4674cb94caeb)

           
  
             
## IDLE TO WALK:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/11f24256-7940-419e-a6e6-e2e81251c139)

           
 
## WALK TO IDLE: 
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/e4364d96-b25b-45f1-8806-689e03ac745c)

 
## WALK TO JUMP:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/677982be-4699-454b-b6fa-b844c9f21c17)

  

## JUMP TO WALK:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/4bd84c0c-5eca-424c-8267-4c43f60c0002)

            
## JUMP TO IDLE: 
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/0e002b1a-a766-4fe0-916f-fddbba960012)

            
## IDLE TO JUMP:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/215ff236-2ccd-42b6-9e0c-1cfb7416a6e9)

            


## ANIMATION BLUEPRINT:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/20c3ab4f-47be-41c7-9066-5371daa65933)

           
            
 
## ANIM MONTAGE:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/e886a54d-2d16-45ce-b35a-694be7f6aca3)


            







## THIRD PERSON BLUEPRINT:
![image](https://github.com/Prethiveerajan/Unreal-EX-NO-3-Change-the-third-person-character-mesh-and-add-animations/assets/94233064/677a9d8e-56d7-46b3-b45d-bf3e144f899a)

          

         


            

## RESULTS:
 The third person character mesh has been successfully changed using animations.




