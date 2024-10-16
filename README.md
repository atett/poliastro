Installed poetry and toml in my base Python 3.10.4 installation for future use

Went back and installed poetry in the PATH so it is callable anywhere

In CMD - 'poetry new xxx' where xxx is the name of the package to create
	in this case, poliastro-testing

pyproject.toml only contains two dependencies, poliastro and simpy
	- poliastros dependencies include numpy and pandas among other libraries
        + Astropy, for physical units and time handling
        + NumPy, for basic numerical routines
        + jplephem, for the planetary ephemerides using SPICE kernels
        + matplotlib, for static orbit plotting
        + numba (when using CPython), for accelerating the code
        + Plotly, for interactive orbit plotting
        + SciPy, for root finding and numerical propagation
	- simpy for setting up time steps for playing with poliastro

poetry install in the folder with pyproject.toml to install the project and create
the virtual environment