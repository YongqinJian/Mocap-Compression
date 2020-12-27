Our code has 5 sections. 
You may run scripts by the following sequence to reconstruct the results
The first section is [Position_Traking],
	run "track_position.py" to get 2d trajectory file "2d_coordinates.txt"
	run "2d_to_3d.py" to convert the 2d trajectories in '2d_coorddinates.txt' to 3d projection and store in the same file

The second section is [3d Modeling],
	run "cut amc.py" can produce sample walk and run files
	run "generate amc.py" can produce the 3d matching run or walk amc file using the "trajectory.txt"

The third section is [PCA],
	run "main.py" would perform our proposed/novel algorithm to code the amc file, and generate "bezier.txt" which is our compressed dataset, "pca.txt" is the plain pca transform matrix

The 4&5 sections are [plot_dof_curves] and [Background Subtraction], This sections are not required for running. The former one is just how we analyze the change of dof over time. you may check those images for more information. And the background subtraction is the background removed video using the online tools