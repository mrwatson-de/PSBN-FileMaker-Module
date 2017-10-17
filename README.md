![Logo](images/PSBN_icon_160x160_sm.png)

# PSBN-FileMaker-Module from mrwatson.de

Ever wanted to Perform Script by Name?

Make FM <-> FM APIs?

Now you can!

:-)

MrWatson
2017-10-18

## Getting Started

* The PSBN Module has been designed to be used as is - just add accounts + security as needed by your system.
* It was developed as a proof-of-concept - to motivate FMI to implement the function natively, and to give developers a chance to see what it can do. 
* It works, so long as the limitations of the technique are not reached - see Limitations below.

Download or clone this repository.

* The **current version** is in the "dist" folder.
* The development version is in the "source" folder.

### Slide shows

Download [MrWatson's Presentation from dotfmp 2017 "FM <-> FM APIs or Perform Script by Name"](http://www.dotfmp.com/file/118)
See the original PSBN presentation in the presentations folder

### Videos

None (Somebody wanna help me here?)

## Release

This is beta quality. Development of a test suite is underway.

Please report bugs here in the Github's Issues.  It would be great if you could provide a fixed version in the issue, with notes, etc.

## Contributing

We welcome contributions from the community. That's what this is all about.

Above all, please vote for a native function [Perform Script [ by Name: ... ] - immediately + natively (Modular-FileMaker)](https://community.filemaker.com/ideas/1187), so that this module can be made redundant!

FileMaker files don't lend themselves well to Github since we can't do merges and pull requests. That's part of what this project is trying to change. But we can still use Github for issues, comments, and planning.

If you find a bug, please include a copy of the file with a Test that shows the bug in action if you can. Its the best way to get your issues addressed.  Bugs that are clearly demonstrated are easily fixed.

If you have a bug fix, please include a copy of the file with the bug fixed. And instructions on where it is.

If you have ideas, please flesh them out in a copy of the file and include it on the issue. Nothing gets an idea across like semi-functional code.

If you have use cases for this functionality, let me know, or post on the Product Idea's page.

## Limitations & known issues

The PSBN module only works for Scripts with internal ID < 4096.

- This is good for 99.9% of files, but old or 'over-scripted' files may go beyond this limit.
  - For example the PSBN file itself is way beyond this limit. 
- Use the "PSBN.GetMaxScriptIDs" script to check if your files are within the limit.
  - Let me know if you are over the limit.

The PSBN module only works for up to 50 different files.

- Should be enough for now

Non exact references to the same file may be treated as separate references.

- For example: "MyFile" and "MyFile.FMP12" are currently treated as separate references.

## Roadmap

- First Version ;-)

Coming:

- First feedback from FileMaker community
- Better example files
- A Test Suite
- (Maybe) A version which supports up to Script-ID 8192

Hopefully coming one day from FMI

- A NATIVE Perform Script By Name function :-)

## Credits

MrWatson - created and designed, and eventually got round to publishing PSBN

Todd Geist - thanks for pioneered the Github thing (I have blatantly ripped this README file from his Generator Github repository)
