---
description: import - Import/reimport animset animation
---

# ▫ Import

## Synopsis <a href="#synopsis" id="synopsis"></a>

```
Usage:
    redmod import -gameRoot=<depot> -inputPath=<file> -animset=<resource-path> [options]​
    
Arguments:
    -gameRoot=<depot>
    -inputPath=<file>
    -animset=<resource-path>
    
​Options:
    -outputPath=<resource-path>
    -animationRename=<name>
    -h, --help
```

## Description <a href="#description" id="description"></a>

The `import` command imports an `.re` animation file into an existing `.anims` animation set file.

Optional parameters include specifying an existing animation name to rename inside the animset file (otherwise the filename of the `.re` animation file is used) or specifying a different output path (default is overwrite).

{% hint style="info" %}
It is best to name `.re` animation correctly even if you replace an existing animation, because the imported animation will always have the filename of the `.re` file.
{% endhint %}

### Arguments <a href="#arguments" id="arguments"></a>

```
-gameRoot=<path>
```

Directory-path to the depot for animset and output (e.g. `C:\modding\depot`)

{% hint style="info" %}
This is the base depot from which relative \<resource-paths> are loaded.
{% endhint %}

{% hint style="info" %}
You need to have the `.rig` file used by the `.anims` animationset present in your depot path.
{% endhint %}

```
-inputPath=<file>
```

Absolute path to the animation `.re` file

```
-animset=<resource-path>
```

Resource .animset file to use

{% hint style="info" %}
Resource path must start with `base\` (e.g. `base\animations\npc\generic_characters\male_average\open_world\generic_male_average__stand__rh_cane_lh_cigar__01.anims`)
{% endhint %}

## Options <a href="#options" id="options"></a>

```
-outputPath=<resource-path>
```

Resource `.anims` file name to write, default is to overwrite the input animset (resource path must start with `base\`)

```
-animationRename=<name>
```

Parameter representing the old name of animation to be replaced by the new animation (default is the filename of the `.re` animation file)

{% hint style="info" %}
The imported animation will always have the filename of the `.re` file even if you specify the animationRename parameter.
{% endhint %}

```
-?|-h|--help
```

Prints out a description of how to use the command.

## Examples <a href="#examples" id="examples"></a>

{% code overflow="wrap" %}
```
redmod import -gameRoot="E:\modding\depot" -input="E:\raw files\animtest1\macarena_long (1).re" -animset=base\animations\npc\generic_characters\male_average\open_world\generic_male_average__stand__rh_cane_lh_cigar__01.anims -output=base\out\new_test.anims -animationRename=stand__rh_cane_lh_cigar__01__smoke__02"
```
{% endcode %}

Imports the animation file E:\raw files\animtest1\macarena\_long (1).re into the animset file E:\modding\depot\base\animations\npc\generic\_characters\male\_average\open\_world\generic\_male\_average\_\_stand\_\_rh\_cane\_lh\_cigar\_\_01.anims and replaces the animation with the name stand\_\_rh\_cane\_lh\_cigar\_\_01\_\_smoke\_\_02 with the name macarena\_long (1). The result is saved to to E:\modding\depot\base\out\new\_test.anims.
