# Pass array jobs to cancel
sacct -X -o jobid,jobname%90 -u rmehta -h | grep jobid | xargs -n 1 scancel
