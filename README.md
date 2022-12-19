# Interactive VR Racing Simulator with IK for PC Powered HMDs

David Buyck

## Abstract

I created a VR racing simulator that has levels of interactivity usually found in videogames. Because of the interaction techniques I classify this project as a Game or Interactive Demo even though my attempt was to make this as realistic as possible. Using the inverse kinematics techniques covered in this course I created an avatar that the user embodies to operate the controls of the racecar [1][2][4]. The inverse kinematics used in this game/simulation use state-of-the-art IK algorithms that efficiently and accurately run-in real time, allowing the rest of the game logic to execute at 100+ frames per second [1]. I also used state-of-the-art VR interaction techniques which allows the user to control the race car with gestures that simulate real race car controls [2][3][5]. The human body animations with the inverse kinematics of the users’ arms allows for a more embodied and immersive experience that is more engaging and compelling for the user [1][2][3][4][5]. 

## 1 Final State of Project

### Click on the images to play the YouTube videos!!!

Intermediate Progress

[![Intermediate Progress](https://img.youtube.com/vi/KqXl652vIJQ/0.jpg)](https://youtu.be/KqXl652vIJQ)

Final Version (4K)

[![Final Video](https://img.youtube.com/vi/ubHl7nM-QQ8/0.jpg)](https://youtu.be/ubHl7nM-QQ8)

Presentation Video

[![Final Video](https://img.youtube.com/vi/7IvLtS4I-bo/0.jpg)](https://youtu.be/7IvLtS4I-bo)

## 2 Key Algorithms, Bottlenecks, and Limiting Factors

Inverse Kinematics are used to reposition and rotate the joints of the user’s avatar to simulate the user interactions inside the cockpit of the race car [4]. I used the Unity Animation Rigging package to seamlessly integrate IK into my project where all the code and algorithms were provided and optimized for the Unity Engine. I used cutting edge interaction techniques to simulate the users’ interactions with the throttle lever and the steering wheel [3]. 

I experienced no bottlenecks in my simulation although bottlenecks would exists if the graphics were improved. The machine I am running the simulation on is top of the line and the IK and interaction techniques are not computationally expensive. The physics are done using the Unity physics engine which is optimized for based on their Data-Oriented Tech Stack. The graphics are light enough to run at 100+ FPS. 

I could improve the graphics of the application but that would require employing an artist or purchasing more expensive assets.  I could add multi-user experiences with photon. Aside from bottlenecking the GPU with more models and detailed environments there is no limiting factors to this simulation on the current hardware. A 100x larger track/world would only have graphical limitations from the level of detail within the virtual world.

## 3 Specific Questions

I was curious if embodiment with IK would improve the immersive experience of VR in a racing simulator. The answer was astoundingly yes! Watch the video and tell me if it seems like a real humanoid is driving that car. I sure felt like I was when I was recording it!

## 4 Initial sketch and progress

![image](https://user-images.githubusercontent.com/47149695/206577408-01cb5760-f8c8-4f51-8621-7bbf51ecb622.png)

![image](https://user-images.githubusercontent.com/47149695/206577450-3472af02-2cfd-46ee-a978-e01100706efa.png)

I made my initial sketch off the racing scene in Ready Player One where Parzival was racing with his VR avatar. I started by bringing in the Unity XR packages and setting up OpenXR input systems so this can run on any OpenXR supported HMD. I think brought in a gender-neutral humanoid model and setup the IK targets to the joints so the IK algorithm can map the body positions with the users hand controllers. I then brought in a car model and used an immense amount of vector math and linear algebra to allow the user to interact with the objects in the vehicle. I created these algorithms myself and did not use any existing packages or algorithms for these interactions. After that I mapped the users’ interactions with car physics and sounds to create the simulation. I had no unexpected changes, and the final project is very close to the sketch I originally made. 

## 5 Peer Feedback

The peer feedback I got from my sketch and intermediate progress was overwhelmingly positive. The graphics, interactivity, IK, and smooth gameplay was noted by my peers. Sound and more interactivity were the only suggestions I had from my peers. I intended to add sound last, which I added, but I did not add any additional interactivity as the implemented interactivity was all I intended to add for this project and the complexity of that alone took the majority of the time for this project’s creation. 

## 6. State-of-the-art elements

The IK package in unity uses state of the art IK that allows the IK to run smoothly and efficiently during a real-time VR simulation in 3D. The interaction and driving techniques in VR are state of the art where the interaction techniques have no documented use in the way I implemented them. I believe there is an opportunity to publish this work, or at the very least use it for a study, after this class is over.

## 7. Future Directions and Limitations

I want to implement foot tracking or pedal controllers in this project. This would allow for realistic gas, brake, and clutch pedal inputs. This would also remove the throttle lever in the center console of the vehicle which currently handles the gas and brake pedal inputs. This would allow me to put a stick shift in the vehicle and I could then implement a gear box which would allow the user to shift gears manually which is commonplace in current gas powered race cars.
 
## References
[1] Ayman Alzayat, Mark Hancock, and Miguel A. Nacenta. 2019. Quantitative Measurement of Tool Embodiment for Virtual Reality Input Alternatives. In Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems (CHI '19). Association for Computing Machinery, New York, NY, USA, Paper 443, 1–11. https://doi-org.ezp1.lib.umn.edu/10.1145/3290605.3300673

[2] Hieu Lê, Tuan Long Pham, and Gerrit Meixner. 2017. A Concept For A Virtual Reality Driving Simulation In Combination With A Real Car. In Proceedings of the 9th International Conference on Automotive User Interfaces and Interactive Vehicular Applications Adjunct (AutomotiveUI '17). Association for Computing Machinery, New York, NY, USA, 77–82. https://doi-org.ezp1.lib.umn.edu/10.1145/3131726.3131742

[3] HyeonBeom Yi, Jiwoo Hong, and Woohun Lee. 2019. DexController : Hand-Held Controller Recognizing Grasp-Pose and Grasp-Force in Virtual Reality Defense Game. In 25th ACM Symposium on Virtual Reality Software and Technology (VRST '19). Association for Computing Machinery, New York, NY, USA, Article 106, 1–2. https://doi-org.ezp1.lib.umn.edu/10.1145/3359996.3365031

[4] Mathias Parger, Joerg H. Mueller, Dieter Schmalstieg, and Markus Steinberger. 2018. Human upper-body inverse kinematics for increased embodiment in consumer-grade virtual reality. In Proceedings of the 24th ACM Symposium on Virtual Reality Software and Technology (VRST '18). Association for Computing Machinery, New York, NY, USA, Article 23, 1–10. https://doi-org.ezp1.lib.umn.edu/10.1145/3281505.3281529

[5] Mohamed Suhail Mohamed Yousuf Sait, Shyam Prathish Sargunam, Dustin T. Han, and Eric D. Ragan. 2018. Physical hand interaction for controlling multiple virtual objects in virtual reality. In Proceedings of the 3rd International Workshop on Interactive and Spatial Computing (IWISC '18). Association for Computing Machinery, New York, NY, USA, 64–74. https://doi-org.ezp1.lib.umn.edu/10.1145/3191801.3191814

## [View the code on Github](https://github.com/davidbuyck/5611FinalProject.git)

This project was made by David Buyck using the Unity Engine with the Unity XR and Animation Rigging packages. I purchased the assets from the Unity asset store.


