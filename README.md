BCI
==============================================

About This Project
----------------------------------------------

A distributed continuous integration script written in the bash scripting
language.

Installation
----------------------------------------------

BCI can be installed on any machine that has Bash and basic unix utilities by
executing the following command:

    $ chmod +x bci
    $ ./bci install ~/.bci

BCI scripts will install to $BCI\_HOME/bin which you should then add to your
$PATH variable

Using BCI
----------------------------------------------

### Adding a Project

The following command will add a project to the BCI projects directory.

    $ bci add some_project https://github.com/some_user/some_project.git

### Removing a Project

The following command will remove a project from the BCI projects directory.

    $ bci rm some_project

### Listing Projects

The following command will list all projects in the BCI projects directory.

    $ bci ls

### Forcing an Update

The following command will force a git pull on the selected BCI project.

    $ bci update some_project

### Forcing a Build

The following command will force an execution of teh configured build command
for the given project

    $ bci build some_project

