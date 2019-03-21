# Example Framer X Project

This is an example of the Framer X folder format currently in beta which allows
you to use your own version control (i.e. git) with your Framer project.

## Checkout

Ensure you have Framer X installed on your machine. Then checkout the project:

    % git clone https://github.com/aron/example.framerfx.git

Ensure that the checked out folder has the `framerfx` extension otherwise
the Framer app will not pick it up. Now just open it in Framer X either by
dragging the example.framerfx folder onto the Application in the doc, using
the **File > Open** menu within the application.

On macOS you can also use the open command:

    % open example.framerfx

Then make changes as needed, and commit them as usual. The standard git process
works for pushing and pulling changes.

## Converting a Project

If you want to convert an existing framerx project to the folder format you
MyProject.framerx:

1. In Finder rename the MyProject.framerx file to MyProject.zip
2. Unzip into a folder called MyProject
3. Rename the folder to MyProject.framerfx

Now you just need to create a git repository within that folder, you can do
so via the command line or using a Git application.

    % cd MyProject.framerfx
    % git init
    % git add .
    % git commit -m "Initial Commit"

You can then push this up to a remote repository on GitHub, BitBucket etc.
