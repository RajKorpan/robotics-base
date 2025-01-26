# Template

This template provides a boilerplate repository
for developing ROS-based software.

## How to use it

Create a new repository on github.com while
specifying the newly forked template repository as
a template for your new repository.

### Place your code

Place your code in the directory `/packages/` of
your new repository.


### Setup launchers

The directory `/launchers` can contain as many launchers (launching scripts)
as you want. A default launcher called `default.sh` must always be present.

If you create an executable script (i.e., a file with a valid shebang statement)
a launcher will be created for it. For example, the script file 
`/launchers/my-launcher.sh` will be available inside the Docker image as the binary
`dt-launcher-my-launcher`.

When launching a new container, you can simply provide `dt-launcher-my-launcher` as
command.
