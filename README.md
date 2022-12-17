# 5611 Final Project
 
David Buyck

VR Racing Simulator 

### Click on the images to play the YouTube videos!!!

Intermediate Progress

[![Intermediate Progress](https://img.youtube.com/vi/KqXl652vIJQ/0.jpg)](https://youtu.be/KqXl652vIJQ)

Final Version

[![Final Video](https://img.youtube.com/vi/7IvLtS4I-bo/0.jpg)](https://youtu.be/7IvLtS4I-bo)

## Key Algorithms

Inverse Kinematics are used to reposition and rotate the joints of the user’s avatar to simulate the user interactions inside the cockpit of the race car. I used the Unity Animation Rigging package to seamlessly integrate IK into my project where all the code and algorithms were provided. I used cutting edge interaction techniques to simulate the users’ interactions with the throttle lever and the steering wheel. To my knowledge no one has done this before, so I implemented my own algorithms and techniques to allow for a smooth and accurate driving simulation.

I experienced no bottlenecks in my simulation. The machine I am running the simulation on is top of the line and the IK and interaction techniques are not computationally expensive. The physics are done using the Unity physics engine which is optimized for based on their Data-Oriented Tech Stack. The graphics are light enough to run at 100+ FPS. 

I could improve the graphics of the application but that would require employing an artist or purchasing more expensive assets.  I could add multi-user experiences with photon. Aside from bottlenecking the GPU with more models and detailed environments there is no limiting factors to this simulation on the current hardware. A 100x larger track/world would only have graphical limitations from the level of detail with the world.

## Specific Questions

Will embodiment with IK improve the immersive experience of VR in a racing simulator? Yes, astoundingly yes!! Watch the video and tell me if it seems like a real humanoid is driving that car. I sure felt like I was when I was making it!

## Initial Sketch

![image](https://user-images.githubusercontent.com/47149695/206577408-01cb5760-f8c8-4f51-8621-7bbf51ecb622.png)

## Presentation

![image](https://user-images.githubusercontent.com/47149695/206577450-3472af02-2cfd-46ee-a978-e01100706efa.png)

I first added a car model. I then added the VR packages. I added the IK packages. I created algorithms to allow for interactivity with the throttle and the steering wheel. I then created algorithms that added physics to the car based on the user’s interactivity. I knew what I wanted to do from before I made the first sketch. The development was steady with continuous debugging and restructuring and refactoring along the way as I learned from my mistakes. 

## Peer Feedback

Feedback was very positive. I made no changes based on peer feedback

## Relationship to State-of-the-Art

The Unity IK packages implement state-of-the-art IK. I also created my own interaction algorithms that are beyond state-of-the-art where no paper has done this before. I plan to publish this work.

## Future Directions

More interactivity could be used in the cockpit. Having a real gearbox would be a grand task but exciting. I had no limitation caused by time. This was a fun project. 

This project was made by David Buyck using the Unity Engine with the Unity XR and Animation Rigging packages. I purchased the assets from the Unity asset store.


