# Set your Camera settings using Python and OpenCV
Here is the shortest python project to change your camera settings (focus, exposure, contrast, brightness) using OpenCV.
It will let you play with all the values to find the right one for your camera model.

**Note:** 
- Based on OpenCV implementation and the camera/webcam driver for your operating system, some settings (called Capabilities) may not be available and adjustable.
- Settings values (direction and range) are highly dependant of the camera manufacturer and model. \
  So you will have to use a trial/error strategy to find the right values for your camera.
  - ie: Higher brightness value could mean brigher or darker image on another camera.
  - ie: contrast=0 could be mean 'normal' contrast or 'very low' contrast on another camera.

# Installation 
```
pip install opencv-python==4.4.0.40
```

#Usage

Start ```opencv-camera_settings.py```
All settings values are shown is the console for you to reuse in other OpenCV project.

## Keyboard shortcuts
| Shortcut | Action |
| :------: | ------ | 
|    S     | Open DirectShow Camera settings|
|    B     | Increase brightness |
|    b     | Decrease brightness |
|    E     | Increase exposure |
|    e     | Decrease exposure |
|    C     | Increase contrast |
|    c     | Decrease contrast |
|    F     | Increase focus |
|    f     | Decrease focus |
|  0 - N   | Switch camera (0 is the default main camera) |
|    L     | Enable live view (Camera will be reserved by this script) |
|    l     | Disable live view (Camera will be usable by other apps while still allowing settings) |

# Samples value

| Camera model   |  Brightness  |   Exposure    |    Contrast  |      Focus    |
| -------------- | :----------: | :-----------: | :----------: | :-----------: |
| Surface book 2
   Front camera  | -130 to +130 |    -2 to 11   | -130 to +130 | Not available |
| Surface book 2
   Rear camera   | -130 to +130 |    -9 to -3.5 | -130 to +130 | 600 (close) to 0 (far) |
| Logitech C270  |    0 to 255  |     0 to -6   |    0 to 255  | Not available |
