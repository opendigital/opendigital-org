## Download RClone

### Installation

Place the executable (after extracting) in a root directory, it can be anything - but you need to make sure to add the executable to the system path variables so you can call it in the CLI.
You can do this by going here: System -> Settings -> About -> Adv. System settings -> Advanced -> Environment Variables. You can also search for this instead.

Under Environment variables, locate the record that says 'path', and click on edit. Select browse and locate the folder where the executable is, and finalize it. For example, the path variable after this should look like this: ```C:/rclone```

Open the terminal and type in ```rclone``` or ```./rclone```. You should see a list of options available when the command is run.

### Configuration

To start config, run the ```rclone config``` command to bring up the configuration prompt. Follow the on screen instructions to link a remote cloud storage. You may set up as many as you'd like provided they have a different name and the right configuration.

### Commands

Commands are traditional linux based commands, consisting of a call, command, and name.
For example, to list flies in a remote called "drive", you would enter the following command: ```rclone ls drive:folder-name```.

*Note*: The ```ls``` and ```lsd``` commands are slightly different. The former lists files recursively in a path, and the latter lists directories, and not the files within them.

Similarly, to download a file locally: ```rclone copy drive:folder-name/path-to-file/file.ext C:/Users/username/Documents -P```.
Note that this command provides a source path: ```drive:folder-name/path-to-file/file.ext```, a space, then a target path: ```C:/Users/username/Documents```; followed by a -P flag, which shows the progress of a download.

Uploading a local file to a remote is much the same, except that you need to swap the source and target with each other, and use the ```sync``` command instead: ```rclone sync local-filepath/file.ext drive:folder-name -v -P```

Use the ```--dry-run``` flag at the end of the command when using sync and copy, so you know what files and folders are being edited and transferred. The ```-i``` flag also creates a prompt before a copy and sync, which creates an additional layer of redundancy.

Deleting files is may also be carried out in a similar manner. ```rclone delete drive:/<folder>/ -P``` or ```rclone purge drive:/<folder>/ -P```. The former command removes all files inside a folder, while keeping the folder itself intact, while the other removes both files and the folder itself.
