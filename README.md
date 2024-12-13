# Dockerfile Bug: Python Dependency Installation

This repository demonstrates a common error in Dockerfiles related to installing Python dependencies.  The original Dockerfile incorrectly installs the dependencies, leading to runtime errors.  The solution demonstrates the correct approach.

## Bug

The original `Dockerfile` attempts to install Python dependencies using `pip3`, but fails because the current working directory isn't correct. 

## Solution

The `Dockerfile_fixed` shows how to correctly install the dependencies and set up the application environment. The WORKDIR instruction sets the correct working directory before installing packages. 