# README #

Incompressible Navier-Stokes problem with Taylor-Green forcing using
the [Dedalus](http://dedalus-project.org) pseudospectral
framework.  To run these problems, first install
[Dedalus](http://dedalus-project.org/) (and on
[bitbucket](https://bitbucket.org/dedalus-project/dedalus)). 

Once [Dedalus](http://dedalus-project.org/) is installed and activated, do the following:
```
#!bash
mpiexec_mpt -n 256 python3 incompressible_NS_TG.py --mesh=16,16
```

For scaling tests on NASA/Pleiades:
```
#!bash
python3 scaling.py run incompressible_NS_TG.py --3D 128 --min-cores=128 --max-cores=512 --MPISGI
```

Contact the exoweather team for more details.

