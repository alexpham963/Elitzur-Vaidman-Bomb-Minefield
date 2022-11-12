# Elitzur-Vaidman-Bomb Quantum Minefield

Hello! This is team Elixer Vitamin Boomers! Quantum Computing Project for the 2022 Fall Fest Quantum Computing Hack-a-thon!

**Brought to you by: Nathan, Chris, and Alex**

#### Video presentation of our Project: https://www.youtube.com/watch?v=p49tTKsIntY

## **PROJECT DESCRIPTION:**
Our project is meant to demostrate a quantum thought experiment known as the Elitzur-Vaidman Bomb Detector but with a fun twist!
Our project is a take on the classic game, Mine Sweeper, where the payer now has to use quantum computation to detect if the mines already revealed on the board are live or not.

## **GAME DETAILS:**
The player is given a 8 x 8 grid filled with 8 randomly placed mines which are indicated by X's. The goal of the player is to use the 
               quantum bomb detector in order to deterime whether the mine is armed or not, and disarm all of the live mines while leaving the duds alone. 
               The player has only 4 attempts to disarm all of the mines. 
               
However there's a caveat, the player is given 100 points which determine how carefully the detector will inspect the mine while making sure 
               it doesn't trigger the mine. 
               If by any chance the user runs out of points before disarming all of the live mines, they now have to disarm 
               the mines blind not knowing if they're duds or live. 
               This forces the player to be strategic about how they use the detector, like for 
               instance using less points on detecting mines that the user thinks are duds.
               
When running the detector, a secondary window pops up which shows the detector's results for that partcular mine with three possible 
               outcomes. The first being that the mine is in fact armed but wasn't triggered, this is the most desirable outcome for the user since it 
               reveals a mine that is supposed to be disarmed. The second outcome is that the result returns a dud. And finally the third and least 
               desirable outcome which is that the mine is armed and that it detonated, causing the player to lose the game. 

## **HOW IT WORKS:** 
### What's the Elitzur-Vaidman Bomb Detector?
The Elitzur-Vaidman bomb detector was a thought experiment created by two Israeli scientists, Avshalom Elitzur and Lev Vaidman, they proposed a 
    scenario where you are given a container that may or may not contain a light-sensitive bomb. Under normal circumstances, the way that you test the 
    container is by firing a single photon at the container and see whether or not it explodes, showing that there was in fact a bomb. However the problem 
    with this is that well... the bomb exploded, which isn't ideal. 
    
However what if you want to find out there's a bomb present and armed without it exploding? Elitzur and Vaidman concluded that you could in-fact find 
    out the bomb is present without exploding it by using superposition. Putting the photon into superposition means in a sense that the photon is in a 
    limbo state where there's a chance that the photon is going either along the upper path of the system or the lower path which is where the container is 
    at. This limbo state is 'collapsed' which means the photon is out of super position and is definitvely in one position or another. Collapsing the 
    photon's superposition is done by observing or measuring the photon which occurs when the container has our bomb inside.  

### Demonstration
![final_6355f3e24b3dfd009908110c_233212](https://user-images.githubusercontent.com/116322729/201489842-92dc2933-2e78-42f8-bfe8-32c51a7e2f7a.gif)
    
As shown by the video demonstration under normal circumstances, our photon gets put into superposition, reaches the top right corner gate the photon 
    gets put out of superposition and then it is detected by only one of the detectors. Reason for this is because the top-right corner gate is known as a 
    Hadamard gate and it returns objects in superposition back to their original state. Meaning it will always be detected by one particular detector. 
  
  ![final_6355f531143b7900d1ad4ab0_318943](https://user-images.githubusercontent.com/116322729/201489847-e547d481-f742-44f4-b6db-bf42ad3c00bb.gif)
    
But when the bomb is placed, our photon is prematurely 'measured' and it's superposition collapses leading it to two possible cases: either the photon 
    collapses to the upper track, or it collapses on the bottom track. The first case can allow us to have knowledge of the bomb's prescence without 
    triggering the bomb; whilst the second case causes the bomb to trigger and no photons are detected in our readers. Both of these cases each have a 50% 
    chance of occuring.
    
There's a reason why I said our first case CAN give us knowledge about the bomb's prescence, this is because there is still that top right corner 
    Hadarmard gate which will put our particle back into superposition and make it so that the photon will be detected in either detector. 

So in this system there are 4 possibilities:
  - No bomb is present and photon is detected in default detector (no bomb): 25%
  - Bomb is present but no photon is detected (bomb blew up): 25%
  - **Bomb is present and photon is detected in default detector (bomb didn't blow up): 25%**
  - photon is detected in alternative detector (unsure): 25%

The last possibility is one where we remain unsure of the prescence of the bomb and need to run the test again. Reason this occurs is because when the 
    bomb causes our photon to collapse it's super position, it leads to the photon being put BACK into superposition and so that means there's a chance the 
    photon will get detected by the alternative detector rather than the intended default detector.

### Improving our odds with Quantum Zeno Effect
With our current system, there's a 25% chance of knowing there's a bomb present without blowing it up. An improvement from the 0% chance under normal 
    circumstances. But what if we want better odds than this? This is where the Quantum Zeno effect comes in!

![final_6355f1c301a0a30083df9754_324325](https://user-images.githubusercontent.com/116322729/201494903-4091c1c6-32dc-46f3-b52e-7a8ea0ec4efc.gif)

The Quantum Zeno effect is a way to manipulate the probability of the superpositioned photon collapsing to a position that won't blow up the bomb if 
    found. In the video demonstration, you can notice that each time the photon goes through each Hadamard gate it sticks to that upper path most of the 
    time. Ensuring that the bomb is detected without blowing it up. In our game, we have it so that the points that the player uses is really just them 
    using the Quantum Zeno Effect.

Credits for the video clips: https://www.youtube.com/watch?v=fus1nJ6JaTk
