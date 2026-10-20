Ox-utils
========

Ox-utils is a collection of various django utilities allowing to reuse them over different
projects. It initially extracted from the `Oxylus Project <https://github.com/oxylus-tech/oxylus>`_.


Features:

- ``ox_utils.conf``: define a Settings class that allows explicit and documented settings and using django settings. Support for dynaconf.
- ``ox_utils.jwt``: JWT tokens encoder/decoder using pyjwt.
- ``ox_utils.models``:
    - Various common models providing common fields, as ``Named``, ``UUID``, ``Color``. 
    - SaveHook: hooks on save and batch save / delete / etc.
    - Owned: wraps over django-caps for parent-child object
    - TreeNode: improved tree models inspired by MPPT.
- ``ox_utils.files``:
    - abstract file and folder models
    - file type detection based on content and create preview from files;
    - support for images, document files as odt, word, pdf;
    - extensible to support custom file types;
- ``pydantic``:
    - currently only add field type to support django lazy translation;
    - to certainly come at some point: django model field de-serializing data using pydantic models;

