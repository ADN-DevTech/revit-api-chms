# Revit API Windows Help Files (.chm)

A collection of the Revit API CHM Windows Help Files from the Revit SDKs.

_Because sometimes you just want that .chm file without having to download and install each SDK_.

This repository shares the RevitAPI.chm Windows help file provided by the Revit SDK for all Revit API releases reaching back to Revit 2012.

These files are used to generate the online Revit API documentation
resources [revitapidocs.com](https://www.revitapidocs.com/)
and [apidocs.co](https://apidocs.co/) that
provide web presentations of the same content.

You should probably use them instead wink wink.

If you are interested in the complete Revit SDKs, please refer to the collection in
the [RevitSdkSamples repository](https://github.com/jeremytammik/RevitSdkSamples).

### Processing the `CHM` Source `html` Snippets

The CHM source source `html` snippets cannot be processed directly with command line tools such as `grep` due to their sheer number:

```
% grep x *htm
zsh: argument list too long: grep
```

Instead, a text file `filenames.txt` containing a list of all the HTML filenames can be generated using `ls`.
That list can be read to process the files easily one by one using a Python script such
as [chmhtmextractor.py](https://github.com/jeremytammik/chmhtmextractor) or other tools.

### LFS

Due to the growing size of the CHM files, we were forced to turn on
the [Git Large File Storage (LFS)](https://git-lfs.github.com/) and move the repository to a new location in the ADN-DevTech organisation
at [github.com/ADN-DevTech/revit-api-chms](https://github.com/ADN-DevTech/revit-api-chms).

### Credits
This repository is a fork of [gtalarico/revit-api-chms](https://github.com/gtalarico/revit-api-chms). The content was moved to a ADN-DevTech repository due to cost associated with hosting LFS.


### Disclaimer

Content is provided free of charge for education and information purposes.

Revit®, Autocad®, Autodesk Inventor®, Navisworks®, DWG™, and associated logos are trademarks and registered trademarks of Autodesk, Inc., and/or its subsidiaries and/or affiliates. All other trademarks, service marks, trade dress, and logos used on the Service are the trademarks, service marks, trade dress, and logos of their respective owners.

Details on using Autodesk trademarks can be found [here](https://www.autodesk.com/company/legal-notices-trademarks/trademarks/autodesk-inc).
