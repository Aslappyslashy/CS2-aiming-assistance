# CS2-aiming-assistance based on yolov8

This is a CS2 assitance designed for fast and accurate head shots, it depend on visible recognion through yolov8, no reading memory or modifying files.



Not packed, if yu want to try, go to the main.ipynb

To start the assistance, execute the first block, and then the fith block of code, there is a few prams you can modulate here:

  rate: the rate where the mouse moves, CS2 locked mouse movment for pydirectinput so I have to use the       win32 mouse movement command, which made the mouse movement undirectional, so, if your assitance are       aiming to slow, increase the rate, or otherwise.
  
  y-rate = this is modulating the pos of mouse with respect to the position of bot's head, when here is       the modulation equation:
    y_pos = k/y_rate, and y_rate can be both positive and negative
  
  accuracy: My code provides a auto fire option, which will only fire when the center of the screen is         with in +-accuracy pixels, so if your auto fire do not work well, increase the accuracy
  
  delay_after_shot: the delay time after every time the assistance autoshots (seconds)
  
  delay_after_detection: the delay after every time it detects, no recommaned to decrease it lower that       0.01 (seconds)
  
  confidence: this is the modulation of yolov8 detection, if your assistance kept firing at sky, objects,       ect, increase the confidence, but, with increasing, it will not detect people further away.I               recommand smaller than 0.7.  

My model provides a valid method of seperating CT and T, but it is not coded yet.
