# pcl_visualizer
Visualizer for a 3D point cloud using PCL Library 1.8...1.12.1

----------------------

This program display a PCL viewer for input point cloud data

## Input file structure support
| Format      | Description |
| ----------- | ----------- |
| .pcd      | Point Cloud Data file format       |
| .ply   | Polygon file format        |
| .txt   | Text file format        |
| .xyz      | X Y Z Text file format       |


## Example
![Screenshot from 2022-06-03 08-21-25](https://user-images.githubusercontent.com/35694200/171862553-c287954b-1a58-4005-8831-c035924ee57f.png)
![Screenshot from 2022-06-03 08-26-18](https://user-images.githubusercontent.com/35694200/171863365-5e259039-7980-47fa-a4ef-34ac20e8db6d.png)
![Screenshot from 2022-06-03 08-31-38](https://user-images.githubusercontent.com/35694200/171864244-aac54f80-6bb0-4ec5-ab0c-e19f669163a1.png)

## Help
```
| Help:
-------
          p, P   : switch to a point-based representation
          w, W   : switch to a wireframe-based representation (where available)
          s, S   : switch to a surface-based representation (where available)

          j, J   : take a .PNG snapshot of the current window view
          c, C   : display current camera/window parameters
          f, F   : fly to point mode

          e, E   : exit the interactor
          q, Q   : stop and call VTK's TerminateApp

           +/-   : increment/decrement overall point size
     +/- [+ ALT] : zoom in/out 

          g, G   : display scale grid (on/off)
          u, U   : display lookup table (on/off)

    o, O         : switch between perspective/parallel projection (default = perspective)
    r, R [+ ALT] : reset camera [to viewpoint = {0, 0, 0} -> center_{x, y, z}]
    CTRL + s, S  : save camera parameters
    CTRL + r, R  : restore camera parameters

    ALT + s, S   : turn stereo mode on/off
    ALT + f, F   : switch between maximized window mode and original size

          l, L           : list all available geometric and color handlers for the current actor map
    ALT + 0..9 [+ CTRL]  : switch between different geometric handlers (where available)
          0..9 [+ CTRL]  : switch between different color handlers (where available)

    SHIFT + left click   : select a point (start with -use_point_picking)

          x, X   : toggle rubber band selection mode for left mouse button
```

## Compilation
This program depends on PCL, VTK and OpenGL.

1. In the root folder create a build directoy

```
mkdir build
```
2. Create compilation files
   
```
cd build && cmake ../src
```
3. Compile project
   
```
make
```

Expected output

![Screenshot from 2022-06-03 08-35-43](https://user-images.githubusercontent.com/35694200/171864937-91aa8a3d-8bff-4f08-a3f8-d084a6243b5c.png)
       
        	 
## Test
```
./pcl-visualizer <cloud file> 
```
Expected output

![Screenshot from 2022-06-03 08-39-30](https://user-images.githubusercontent.com/35694200/171865601-c64efd17-a088-4f3f-afda-c62d20d04f93.png)

## Docker
There is an docker image in process for this project...
