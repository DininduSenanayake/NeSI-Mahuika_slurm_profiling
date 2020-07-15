### NeSI-Mahuika slurm profiling

<span style="font-family:Cambria">
  
This is to be used n an instance where it is necessary to examine resource usage (cpu, memory, I/O , cumulative I/O over the run-time of your job. The data is collected into a file on a shared file system for each step on each allocated node of a job and then merged into an HDF5 file. 

* add `#SBATCH --proflie task` to batch submission script
* On completion of the job, create the .h5 file via `sh5util -j jobid`
* Generate the .png file with `python rofile_plot_Jul2020.py filename.h5`
</span>
