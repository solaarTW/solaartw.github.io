---
description: Vehicle assets
---

# ▫ Assests

## Brief

Listing of vehicle assets needed for vehicles to be vehicles

## Asset Files

### .ent File (entEntityTemplate)

This file contains a list of the different appearances, along with the default. Each item in the appearances list contains the fields below, and the defaultAppearance can be set to random, or any of the appearanceNames defined in the list.

| Key                | Example Value                                              |
| ------------------ | ---------------------------------------------------------- |
| name               | quadra\_type66\_\_basic\_urban\_01                         |
| appearanceResource | `base\vehicles\appearances\sport\quadra_type66__basic.app` |
| appearanceName     | urban\_01                                                  |

### .app File (appearanceResource)

This file defines the resources needed for each of the vehicle's appearances. Some important fields are below:

#### appearanceResource

* baseEntityType: name that exists in the Base Types Map and mapped to the correct .ent file
* commonCookData: the .cookedapp file that stores a copy of the data for faster loading

#### appearanceDefinition

* name: the appearance's name that is listed in its .ent file
* parentAppearance: the appearance this one inherits information from
* proxyMesh: the .mesh file loaded for rendering the vehicle at a distance (confirmation needed)
* resolvedDependencies: resources loaded right away (confirmation needed)
* looseDependencies: resources loaded lazily (confirmation needed)

