# VL

## Overview

* The most important components of VL are *_Nodes_* and *_Links_*.
* Nodes and links live on a canvas called *_Patch_*.
* One or multiple patches are contained in a *_VL Document_*. VL Documents are stored as files on disk.
* Every patch can define one or more *_Operations_*. Operations can be created as nodes in other patches.
* There are two kinds of patches, one is merely a container for independent operations the other is a data type. If a patch is a data type its operations can store and/or share data via *_Properties_*. Properties can be accessed and/or modified in operations via *_Pads_*.
* One _VL Document A_ can reference another _VL Document B_ to use its data types and operations as nodes. File B is then called a *_Dependency_* of A.
* Patches can also contain *_Regions_*. A region defines a new computational context. There are different kinds of regions.
* Nodes and regions can have inputs and outputs called *_Pins_*.
* Static data can be entered into an operation using *_IOBoxes_*. IOBoxes are little editors for basic types like numbers, text, color… They can also be used to display the current value of anything connected upstream.
* Links transport data from outputs to inputs. Therefore they define the data flow and execution order of the nodes in an operation.
