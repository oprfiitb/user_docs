OpenPOWER Research Facility at IIT Bombay uses the IBM Spectrum Load Sharing Facility (LSF) for scheduling the jobs

Submitting a job
----------------
To submit a job, use
``bsub -q "queue_name"(short|normal) -n total_no_of_cores(N) -R resourcetype(cs|gpu|capi)  -W walltime (HH:MM) -J jobname -j jobfilename``

Queues
~~~~~~
We currently provide two queues:

* Short

  This is for short usage. Less than an hour.

* Normal

  This is for long usage. More than an hour

Total No of Cores
~~~~~~~~~~~~~~~~~

Here, you provide the total number of cores you will use. 

Look at each node to see the number of cores available. 

Resources
~~~~~~~~~

The OPRF Cluster provides various kind of resources along with the POWER8 CPU Power. 

Read each node's information to see the type of resources available on it.

Walltime
~~~~~~~~

Wall time is your estimate of how long a job will run. Once your job exceeds this time limit, it will stop.
If you don't specify the wall time, it is unlimited by default.

Jobname
~~~~~~~

Name for the job for reference purposes.

Jobfilename
~~~~~~~~~~~

You can put all the info about the that you gave *bsub* in options, along with the various steps required to execute the job inside a single file and then give that file to *bsub*.

Once you have submitted a job
-----------------------------
``bjobs -l jobID``
If submited succesfully *bsub* will return a jobID with the queue in which the job is submitted.

For history about the submited job, use
``bjobs -l jobID``

For information about *all* jobs you have submited, use
``bhist jobID``

Further reading
---------------
For more help on using LSF scheduler please refer to the following links
1.http://research.computing.yale.edu/hpc-support/user-guide/lsf
2.https://www.ibm.com/developerworks/community/wikis/form/anonymous/api/wiki/99245193-fced-40e5-90df-a0e9f50a0fb0/page/22e9aefe-a2e8-46e6-ad62-2ff5860f45aa/attachment/f8aad44b-8e1c-4051-95c9-d2c80fe90cf3/media/lsf_command_ref.pdf

