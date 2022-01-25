# one of the key problems in computer vision is recovering the 3D structure of a scene from its images.

we have a scene that defined in the world coordinate frame when we reconstructed the scene we would like to know where each point lies in the world coordinate frame say as in milimeters.but what we have is the disposal are images of the scene where points are measured in terms of pixels.
In order to go from images to full matrix reconstuction we need two things - 
1. the first is position of the camera with respect to world coordinate frame this are refered as the external parameters of the camera.
2. And then we wanna know how the camera maps via perspective projection point in the world onto its image plane this are refered as internal parameters of the camera (such as its focal length).

so determining the external and internal parameters of the camera is refered as camera calibration.

so we are gonna develop a method for estimating the external and internal parameters of the camera.

before we can do doing this we first need a model of the camera and this is what we refered as camera model or a forward imaging model which takes from 3D to 2D.

# Linear Camera model
which takes a point in 3D to its projection in pixels in the image. linear model is a single matrix called a projection matrix.so now projection matrix in place we develop a camera calibration method.


# camera calibration
we take a single picture of an object of a known geometry this is what we need to fully calibrate the camera in other words to determine the projection matrix.

# Extractiing Intrinsic and Extrinsic Matrices
once we have determine the projection matrix we can actually tear it apart to figure out both the internal parameters and the external parameters of the camera. this are called Intrinsic and Extrinsic Matrices.

At this point the camera is fully calibrated.


# calibration patterns
sometimes known as a calibration grid or a calibration target is a repeating pattern of known size and spacing. for example checkerboard pattern consists of alternating white and black squares of equal size.

# checkerboard pattern
camera calibration using checkerboard pattern to get the Intrinsic Matrices depends on the camera calibration accuracy.






	

