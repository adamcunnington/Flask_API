# Flask_API

Flask's documentation describes that the "micro" in microframework means Flask aims to keep the core simple but extensible, and that Flask won't make decisions for you. In other words, Flask is not opinionated.

In contrast, Flask_API is very opinionated. Flask_API is a Flask extension that provides a foundation for building Web APIs. It is more than boilerplate - it is designed to contains all the tools needed to build a scalable Web API, as per the author's opinions. It is "RESTful" in the sense that the Author advocates REST principals and implements them when deemed feasible.

Flask_API is being built predominantly for the [Convention](https://github.com/adamcunnington/Convention) project - to decouple the generic API functionality from application specific code. Whilst not primarily built to be distributed, it is recognised that web APIs are incredibly commonplace and Flask is an increasingly popular framework. Therefore, this project is open source, allbeit not stably supported.


***

## Features

The following list of features is not extensive but will guide the development effort:
- Extendable Flask_SQLAlchemy model
- Versioning (resources and model)
- Authentication / Authorisation (distinction TBC); OAuth2 but active directory supported need (SAML2?)
- Endpoint decorators:
    - JSONifying
    - Pagination
    - Cache Control
    - ETag
- Error handling
- Resource documentation
- Python abstraction layer for making requests

This project is currently in the design / early development phase.


***

## Installation

The following installation steps assume that you have cloned the master branch into *C:\Python Projects\Flask_API*:
1. [Install Python](https://www.python.org/downloads/ "Download Python"). Tested with 3.6.1 but there's no known reason why this won't work in any python build >= 2.7.
2. Create a virtual environment. If you are using Python 3.3 or later, use [pyvenv](https://docs.python.org/3/library/venv.html "Python 3 Docs: venv"), otherwise, use [virtualenv](https://pypi.python.org/pypi/virtualenv "PyPI: virtualenv").
3. Activate your virtual environment.
4. Change directory into *C:\Python Projects\Flask_API* and Install flask_api with:
```
python setup.py install
```
