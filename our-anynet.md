version information for our-AnyNet-master

-----------------------------------------
version : 1.0
update time: 2020/3/2 by yhy

1. for pytorch>=1.0
2. be sure to do in a new environment:
    '''
    cd models/spn_t1
	  bash make.sh
    '''
   search "AnyNet" in github for more details.
3. together.py:
	mode = 1  for  resolution:1280x800
	mode = 2  for  resolution:640x400
	see 4. followed !
4. new stereo rectify configures in config_matlab.py for resolution of 640x400
	1.chess23s------chess2+chess3 stereo_calibration in MATLAB (good performance)
	2.chess2s------chess2 stereo_calibration in MATLAB (best performance)
	3.chess3s------chess3 stereo_calibration in MATLAB (bad performance)

To rebuild the project:
be sure to include : 
	together.py
	Get_Depth.py
	camera_use.py
	utils/data_from_camera.py
	stereo_calibrate(note : the whole folder)

------------------------------------------------
version : 1.1
update time: 2020/3/2 by yhy

1. modify three files:
	1. together.py 
	2. Get_Depth.py
	3. utils/data_from_camera.py
2. new input args:
	args.Mode (Mode 1:(1280x800)  Mode 2:(640x400)  default=2)
	args.with_spn (default=True)
3. note that I made the :
	output_depth = output/np.max(output)
    the denominator above also can be 256
