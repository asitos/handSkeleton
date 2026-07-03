# handskeleton

just a little experiment using mediapipe to turn my hands into a 3d-connected mess. it tracks both hands and draws lines between the fingertips, creating a kind of glowing web between them, with some simple depth math added, so the lines get thicker and brighter as you bring your hands closer to the camera.

## getting it running

1. make sure you have python and pip installed.
2. install the requirements:
   `pip install opencv-python mediapipe numpy`
3. grab the `hand_landmarker.task` file from [google's mediapipe repo](https://storage.googleapis.com/mediapipe-models/hand_landmarker/hand_landmarker/float16/latest/hand_landmarker.task) and drop it in the same folder as this script.
4. run it: `python handLandmarker.py`

--- 

it’s pretty straightforward—it looks for two hands, identifies which is left and which is right, and then starts drawing. if it's struggling to see both, it'll let you know in the hud. just hit 'q' when you're done playing with it.

i attended a workshop held in my college which helped me understand opencv, mediapipe, and basic python, with a pretrained hand_landmarker.task model from google's mediapipe repository.

---

## a fun note
i learned more about vim basics, and how plugins like black help with lazyvim to code in python and get it running, since i didnt want to use vscode or any heavy ide, which helped me learn:

1. how buffers, windows and tabs work
2. open multiple files and navigate through them
3. open a terminal inside nvim, and run python code within it 
4. using hyprland tiling layouts to my advantage and have my code and documentation side by side
