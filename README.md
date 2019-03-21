# Example Framer X Project

This is an example of the Framer X folder format currently in beta* which allows
you to use your own version control (i.e. git) with your Framer project.

[Framer Folder Format Documentation ›](https://framer.gitbook.io/teams/integrations#folder-projects)

\* As a beta feature it is strongly recommended that you only use this format with
version control.

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

If you want to convert an existing `framerx` project to the folder format you
can do so by going to **File > Save As** and selecting "Framer X (Folder)".
You'll need to hold the <kbd>option</kbd> key for the **Save As** menu item
to appear.

Now you just need to create a git repository within that folder, you can do
so via the command line or using a Git application.

    % cd MyProject.framerfx
    % git init
    % git add .
    % git commit -m "Initial Commit"

You can then push this up to a remote repository on GitHub, BitBucket etc.
