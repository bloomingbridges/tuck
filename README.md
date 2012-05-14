tuck
====

I love myself an __empty__ desktop. If you require yours to be ruled by chaos, then __tuck__ is not for you.

Likewise do I feel about sorting stuff into folders. While this process could in theory be automated, I'd rather have complete control over what goes where and I want that process to as quick as possible i.e. not using drag and drop.

### May I introduce __tuck__?

__tuck__ is a command line tool - written in Ruby - for filing your incoming clutter into predefined folders.

Whenever you call __tuck__ he goes through your "busy" folders (by default that would be 'Desktop' and 'Downloads') and asks where to put each file (not folders!), to which you reply with a single character. You're welcome :>

### Usage

1. First copy __tuck__ (including the configuration file 'tuck.config.yaml') into a folder that's easily reachable e.g. your home directory.

2. Add folders to watch and destination-key pairs to 'tuck.config.yaml' with a regular text editor.

3. Open a new Terminal window, navigate to the directory __tuck__ sits in and invoke him as follows:


    ./tuck

	# Or make use of the '-p' option to show a QuickLook preview for every entry:

	./tuck -p

4. For each encountered file enter the character corresponding to the desired directory and confirm by hitting return. Is no character given the file will be skipped, a single space will stop the script completely.

Happy tucking!

### Future plans

The idea is to eventually turn __tuck__ into a commercial Cocoa application. However, on top of the basic functionality __tuck__ currently offers one can expect the following features to be added in the near future:

* Make it cross-platform (currently OS X/UNIX[?] only)
* Add a dialog for moving the current file someplace else completely
* Blacklist for watched directories so folders can also be tucked
* Make it possible to define rules (RegExp) for handling similar files