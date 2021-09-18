# Installing the minimum required XCode command line tools to run Git

## The "invalid active developer path" error

If you attempt to run git on MacOS and get an "invalid active developer path" error message like this then you need to install the XCode command line tools. 

```
$ git

xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun
```

## How to install XCode command line tools without the rest of XCode

You can install XCode but it's a huge download. You can save about 80% of the disk space by installing the command line tools alone. 
Here's how.

* Run `xcode-select --install` from the command line:

```
$ xcode-select --install
```

A dialog appears with a message something like this: `The "xcode-select" command requires the command line 
developer tools. Would you like to install the tools now? Choose install to download
and install the command line developer tools now."

* Click the Install button.

You're asked to agree to license terms and so forth. 

* Click the remaining permissions dialogs and wait for the "Downloading software" and "Installing software" dialogs to complete.

It should take several minutes at least.



