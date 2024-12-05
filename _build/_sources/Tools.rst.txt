Tools
=====

Here are some common tools WIP

**make longer**


Containers
----------

Portable, fully encapsulated environments that bundle an application with all its dependencies, including libraries and the operating system. They ensure that applications can run consistently across different systems, regardless of the underlying hardware or software configurations.

Key Features : 
^^^^^^^^^^^^^^
* Provides a complete and portable environment for running applications
* Useful for deployment and cross-platform development.
* Often used in production and cloud environments (Docker)

Add Demo Here

Conda
-----

An environment and package manager that allows users to create isolated environments not
only for Python but also for other languages. It’s especially useful for data science and 
machine learning projects that rely on multiple tools across different languages

Key Features : 
^^^^^^^^^^^^^^
* Allows installation for both system-level and Python-specific packages
* Can handle non-Python projects, making it more versatile than virtual environments.


Virtual Environments
--------------------

Used to create isolated environments for Python projects only. They are a way to separate 
dependencies of different python projects to avoid conflicts.

Key Feartures : 
^^^^^^^^^^^^^^^
* Only manages Python libraries
* Does not manage system-level (OS) dependencies
* Idea for small-scale projects or situations where you only need to isolate Python dependencies

Add Demo Here

Pip
---

Default package manager for Python. It installs libraries directly into the environment, 
but unlike Conda or Containers, it does not idolate or manage the dependencies themselves. 

Key Features : 
^^^^^^^^^^^^^^
* Installs Python libraries into the active environment.
* Typically used alongside Virtual Environments or Conda to install dependencies.
* Doesn’t manage system-level dependencies or environments.
