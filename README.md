BCI
==============================================

About This Project
----------------------------------------------

A distributed continuous integration script written in bash script.

Installation
----------------------------------------------

BCI can be installed on any machine that has Bash and basic unix utilities by
executing the following commands:

    $ BCI_HOME="$HOME/.bci"
    $ mkdir -p "$BCI_HOME"

BCI scripts will install to $BCI\_HOME/bin which should then be added to your
$PATH variable

Using BCI
----------------------------------------------

### Adding a Project

The following command will add a project to the BCI projects directory.

    $ bci add some_project git@github.com:some_user/some_project.git

### Deleting a Project

The following command will delete a project from the BCI projects directory.

    $ bci del some_project

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

