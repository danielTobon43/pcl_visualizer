# pcl_visualizer
Visualizer for a 3D point cloud using PCL Library 1.9.1 

----------------------

This program display a PCL viewer for input point cloud data

## Input file structure support

* .pcd 
* .ply
* .txt
* .xyz


## Example

<img src="./example/example.png" align="center" height="500" width="900"><br>

## Compilation
* Set "YOUR OWN" PCL Build DIR in CMakeList.txt e.g: **/opt/pcl-1.9.1/build** and save it.
* Create a "build" folder

in the main folder:

	- cd /build  
	- cmake ../src/
  	- make
       
        	 
### Test

	cd /build/bin
	./pcl-visualizer <cloud file> 
