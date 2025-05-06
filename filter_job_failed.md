# Which ones failed
sacct -n -X -o state%20,jobname%90,jobid%20 -u rmehta | grep FAILED

# Number failed
sacct -X --starttime 2021-05-03 -o state%20 -u rmehta | sort | uniq -c 
