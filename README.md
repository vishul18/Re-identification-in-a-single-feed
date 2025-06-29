# Re-identification-in-a-single-feed
Aim - 
Given a single 15-second video clip (single camera angle), detect all players and assign each a consistent player ID, even if they temporarily leave the frame and reappear later.
Approach - 
I used two part pipelines , First I did player detection with the help of the pre made fine tuned yolov11 and the detection threshold was selected 0.4 for the accuracy to be as precise as required. The focus was kept on the players and Then i did use deepsort to assign the id's for the players and DeepSORT uses both motion and appearance features to re-identify players when they re-enter the frame and Hyperparameter was used to keep the Id's from getting switched.
Files Involved - 
a)best.pt - Pre trained Yolov11
b)15sec_input_720p.mp4 - Input Video
c)player_tracking_fixed.mp4 - Output Video
Output - 
In the final output video You can see the player with the id's.
