# Boiler

Boilerplate directory structure for your Github Projects!

## Purpose

The inspiration for this project came after perusing this repository: 
- https://github.com/kriasoft/Folder-Structure-Conventions

When starting new projects and repositories, boilerplating the project directory structure is a pain in the butt.
It would be great to have a simple way to start a project with a sane default directory layout.

This project intends to provide just that!

## Usage

Try something like this (bash syntax):

```
git clone --depth=1 --branch=master <a link from the "clone or download" button>
rm -rf boiler/.git/
mv boiler/ <your new project's directory name>/
cd <your new project's directory name>

# optionally: clean out .gitkeep files
find . -name .gitkeep -delete

git init
```

Now you're ready to Rock and Roll!

## Directory Layout

```
.
├── src                     # Source files (alternatively use `lib` or `app`)
├── lib                     # Libraries and module sources
├── 3P                      # Third party Libraries and modules
├── build                   # Compiled files (alternatively `dist`)
├── tools                   # Tools and utilities
├── scripts                 # Useful scripts
├── test                    # Test files (alternatively `spec` or `tests`)
│   ├── benchmarks          # Load and stress tests
│   ├── integration         # End-to-end, integration tests (alternatively `e2e`)
│   └── unit                # Unit tests
├── docs                    # Documentation
│   ├── TOC.md              # Table of contents
│   ├── faq.md              # Frequently asked questions
│   └── ...                 # etc.
├── CHANGELOG.md            # A running list of changes and fixes
├── LICENSE                 # CYA
└── README.md               # $this
```

### License

Use this however you would like for "free, as in beer".
