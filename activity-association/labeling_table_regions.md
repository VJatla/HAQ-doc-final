## Procedure
1. **Create session video:** We first combined all the videos in a session
	taking one frame every second. We call this file, `session_video.mp4`.
	A video that has $`t`$ seconds will contribute  $`t+1`$ frames.

2. **Label bounding boxes:** We then used MATLAB 2021b video labeler to label 
	bounding boxes on `session_vide.mp4` following the [protocol](#protocol). 
	The saved MATLAB session is  `session_roi.mat` which is exported to a mat 
	file, `session_roi_exported.mat`.

3. **Export to CSV:** The mat files are hard to read and process in python. So
	we use the script, `./table-roi/mat_to_csv.mat` to convert to CSV file, `
	session_roi.csv`.

4. **Create video level table-roi:** We now have table regions of interest at
	30x speed. From this we create a csv file that maps the regions back to 
	original videos. We use `session_to_vidoes.py` to create `video_roi.csv`

## Protocol
??? Sravani needs to fill this up.
