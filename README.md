# Orchestrating end-to-end reproducible NextGen and NextGen-adjacent workflows - Part 2: Orchestrating parallel model calibration

The code demonstrations in this workshop can be run either locally on a machine with multiple CPU cores or on the 2i2c workshop hub, which can be accessed at https://workshop.ciroh.awi.2i2c.cloud/hub/login. Your credentials for the workshop hub consist of your GitHub username (or firstname-lastname) and the password available here:

https://vault.bitwarden.com/#/send/PVmSEbW9ukO3xbRCAVHk7w/1PgyxbYP3DynRr20CHm-FQ

Once logged in, start a server with the "Community Assets Computation Hub" image and run the following commands from the server's terminal:

```sh
mkdir -p /home/jovyan/SYMFLUENCE_data
ln -s /opt/symfluence/data/installs /home/jovyan/SYMFLUENCE_data/installs
/srv/conda/envs/symfluence/bin/python -m pip install mpi4py
```

These commands create a symlink to the SYMFLUENCE binaries we will need during the workshop and install mpi4py into the Python environment used by SYMFLUENCE. The CIROH team may have already set up the symlink. If so, the second command will report "File exists", which is harmless and can be ignored.

If you'd prefer to run SYMFLUENCE locally, installation instructions are provided here: 

https://symfluence.readthedocs.io/en/latest/installation.html
