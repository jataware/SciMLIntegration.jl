# SciMLIntegration.jl
One-off modeling operations using SciML under the hood.

This module provides high level functions to be used by [the PyCIEMSS service](https://github.com/DARPA-ASKEM/pyciemss-service). 
`SciMLIntegration.jl` provides a similar interface to what [PyCIEMSS](https://github.com/ciemss/pyciemss) exposes.

Currently, the only available operation is `simulate`. The client service uses [PythonCall.jl](https://github.com/cjdoris/PythonCall.jl)
so it's important that SciMLIntegration only returns types that easily convert to Python.
