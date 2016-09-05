Welcome!
--------
An account for OpenPOWER Research Facility at IIT Bombay(OPRF) grants you shell access to the OPRF POWER8 Cluster. 

To access this cluster you can use the ``ssh`` client available in almost all \*nix distributions like Linux. If you are a Windows user, you can use a software like MobaXTerm_, putty_ or `Bitvise SSH Client`_. We recommend that you gain familiarity with Linux, if you already havne't, to be able to use OPRF effectively.

Once you login on the cluster using the information that you received in the Welcome email from OPRF Team, you will get a shell prompt on a machine called **ipaserver**. This is the machine from which you can schedule your jobs to run on the OPRF.

Your home directory is at `/home/oprfusers/YOUR_USERNAME`.

Inside your home directory you will find following:

* `scratch` directory:
   This directory is for your programs and jobs to use as a temporary scratch space or for storing the results of computation.
* `code` directory:
   This is where you should store your own code or the software that you will compile and install for running on the OPRF. 
* `results` directory:
    Same as `code`. `results` is a symbolic link to the `scratch` directory for convenience.

The above directories each have been granted a different disk usage limit based on observed needs of users. Thus, we strongly recommend that you use the directories for their suitable purposes and do not try and store everything inside your home directory as it has a quota limit too.

Frequently Asked Questions
--------------------------

* A software that I need is not present on OPRF! What should I do ?

  We recommend you install required software and libraries inside the `code` directory in your home directory. We do not provide *sudo* access or administrative permissions to any user and will install a software system-wide *if and only if* we find that a good enough number of users need it.

* How do I copy a file to OPRF? How do I copy a file from OPRF?

  You can use the `scp` command and the same credentials and connection details that you received in your Welcome email. You have complete read and write access over your home directory which you can refer as `/home/oprfusers/YOUR_USERNAME` or `~YOUR_USERNAME`. You can also use the **SFTP** functionality in your SSH Client to copy files to and from the OPRF Cluster.

* How do I download a file from Internet on the OPRF Cluster? How do I clone a github repo on OPRF ? How do I download my software on OPRF cluster?

  Internet access is not available to OPRF Users on the cluster. We recommend you download the files locally, compress them in an archive using ZIP or Bzip2 compression and then copy them to OPRF. If your software is very big, you may request the system administrators for directly downloading it on the cluster.

* My question is not answered here. I need some urgent help!

  Email the OPRF team at `help AT oprfiitb DOT in`


.. _MobaXTerm: http://mobaxterm.mobatek.net/demo.html#
.. _putty: https://www.bitvise.com/ssh-client-download
.. _Bitvise SSH Client: https://www.bitvise.com/ssh-client-download
