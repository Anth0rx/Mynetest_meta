# Mynetest
This is the Mynetest meta repository to use in conjunction with the `repo` tool.

## Getting Started
To get started with Mynetest, you'll need to get familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

### Install the `repo` tool
Either the `repo` tool is available in your distributions repository or you have to install it manually.

#### Manual install:

##### Put the `~/bin` directory in your path of execution
In recent versions of Ubuntu, `~/bin` should already be in your `PATH`. You can check this by opening `~/.profile` with a text editor and verifying the following code exists (add it if it is missing):

    # set PATH so it includes user's private bin if it exists
    if [ -d "$HOME/bin" ] ; then
        PATH="$HOME/bin:$PATH"
    fi

Then, run source `~/.profile` to update your environment.

## Initialize the repository
To initialize your local repository using the mod repositories, use a command like this:

    repo init -u git://github.com/Anth0rx/Mynetest_meta.git -b master

Then to sync up:

    repo sync
    
    
Parts of the README are from the [LineageOS Wiki](https://wiki.lineageos.org/devices/hammerhead/build).
