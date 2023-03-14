simplejwt-clean-django
===

Clean Django Repository to test rest_framework_simplejwt types against.

The rest_framework_simplejwt fork is initialized as a git submodule. Repository link and branch: https://github.com/PedroPerpetua/djangorestframework-simplejwt/tree/improve-typing


## Getting started
1. Clone the repository.
2. Get the submodule (`git submodule update --init --recursive`).
3. Install the dependencies (`pip install -r requirements.txt`).
   - Recommended to do so in a virtual-environment.
4. Run `mypy` to type check the submodule.


## The `/app` folder
The `/app` folder contains a clean django project with **NOTHING**\* changed. This is so it's a blank state to be used by django-stubs as a working point.

\* Added a `type: ignore` comment to `ALLOWED_HOSTS` because it wasn't type and the strict mypy configuration was complaining about it.
