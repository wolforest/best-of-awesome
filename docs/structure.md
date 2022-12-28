

## structure of project "hello":
```
hello/
├── LICENSE
├── bin
│   └── start.sh
├── docs
│   └── README.md
├── hello
│   └── world.py
├── pyproject.toml
└── tests
    └── world_tests.py
```

## __init__.py Best Practices
__init__.py files are used to initialize Python packages. They are executed when the package is first imported.

_init__.py files can be used to set up global variables, define functions and classes, and run code.

While __init__.py files are not required, they are often used to customize the behavior of a package.

1. Use __init__.py to control what is imported by from module import *
2. Use __all__ to control what is imported by from package import *
3. Use __version__ for version numbering
4. Use logging in __init__.py
5. Use __init__.py to define a consistent look and feel for your packages
6. Use __init__.py to initialize the package level logger
7. Use __init__.py to register entry points
8. Use __init__.py to configure matplotlib
9. Use __init__.py to load data files
10. Use __init__.py to set default values for other modules


