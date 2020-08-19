# DBeaver Docksal addon

**NOTE: This repository is no longer maintained!  
The dbeaver script is now part of the [docksal addons repository](https://github.com/docksal/addons).**

This Docksal addon launches [DBeaver][1] with the connection information from the current project.
DBeaver is a multi-platform database tool which supports popular database engines like MySQL, PostgreSQL, SQLite and more. 

This addon tries to detect the database engine and launches DBeaver with the correct connection settings.
Currently only the following database engines can be detected:

* MySQL
* PostgreSQL

## Requirements

* Linux or OSX 
* [Docksal][2]
* [DBeaver][1]

## Installation

### Global

To install this addon globally, clone this repository inside the `$HOME/.docksal/addons` directory.

```bash
mkdir -p $HOME/.docksal/addons
git clone git@github.com:CyberJack/dbeaver.git $HOME/.docksal/addons/dbeaver
```

### Inside a single project

To install this addon inside a single project, clone this repository inside the `.docksal/addons` directory within the project. 

From the root of the project run:

```bash
mkdir -p .docksal/addons
git clone git@github.com:CyberJack/dbeaver.git .docksal/addons/dbeaver
```

## Usage

```bash
fin dbeaver [service_name (default: db)]
```

Run `fin dbeaver` to launch DBeaver with the connection information from the current project. If the database service name is not `db` or the project has multiple database services, a service name can be provided as the first parameter.

## Contributing
Pull requests are welcome. Make sure to use [ShellCheck][3] before submitting a pull request.  
For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Links

* Docksal: [https://docksal.io][2]
* DBeaver: [https://dbeaver.io][1]
* ShellCheck: [https://www.shellcheck.net][3]

[1]: https://dbeaver.io
[2]: https://docksal.io
[3]: https://www.shellcheck.net

