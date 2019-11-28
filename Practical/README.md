[Hands-on slides](https://docs.google.com/presentation/d/1R9nks5vpHQduNcjewRaLr1KDpNLBg-8fN1-PfdhGpXM/edit?usp=sharing)
[Hands-on google doc](https://docs.google.com/document/d/1HKXR65TYYjriV29-EZRXevcEuR8WSTzOTK0cJqXsWPw/edit?usp=sharing)


### Day 3: November 29th

**Start at 8H30**

**Location:** Salle Shannon - Maxwell Building - Place du Levant, 3, Louvain-la-Neuve  ([google map](https://goo.gl/maps/UYkweqZo7QsLxbyWA))


#### Morning and afternoon: Mohamed + Remi + Olivier

[Hands-on slides](https://docs.google.com/presentation/d/1R9nks5vpHQduNcjewRaLr1KDpNLBg-8fN1-PfdhGpXM/edit?usp=sharing)
[Hands-on google doc](https://docs.google.com/document/d/1HKXR65TYYjriV29-EZRXevcEuR8WSTzOTK0cJqXsWPw/edit?usp=sharing)

**Hands On**

- How to design your fMRI experiment
- Exploring a BIDS data set
- Preprocess
  -   Slice timing
  -   Realign & coregister
  -   Normalize
  -   Smooth

-   Lunch: 12H00 - 13H00

-   Subject level GLM
-   Group level GLM
-   Stats - correction
-   Looking at group level results
-   How to batch / script your analysis


___
## Practical information


### What you will need

For the hands-on part, it is mandatory that you come with your own laptop and have the following things on it:

-   5 gigabytes of free space to comfortably run the analysis
-   Matlab
-   [Atom text editor](https://atom.io/)
-   [MRIcron](https://www.nitrc.org/projects/mricron/) and [MRIcroGL](https://www.nitrc.org/frs/?group_id=889) for the easy visualization of MRI images
-   [SPM12](https://www.fil.ion.ucl.ac.uk/spm/software/download/)
-   Code for the automated analysis pipeline from the CPP lab (from [zenodo](https://doi.org/10.5281/zenodo.3554332) or get the latest version from [github](https://github.com/cpp-lln-lab/CPP_BIDS_SPM_pipeline/releases) )
-   Data we will be using for the practical:
  -   for preprocessing and subject level analysis: the `raw_additional.zip` from this [zenodo repository](https://doi.org/10.5281/zenodo.3548325)
  -   for the group level analysis: the `derivatives_group.zip` from this [zenodo repository](https://doi.org/10.5281/zenodo.3548325)

Further information on installation and updates will be posted [here](https://github.com/cpp-lln-lab/fMRI_workshop_201911)

If you have trouble with installing any of those, we can also help you set those up in the 2 days prior to the practical.


### Installing SPM12

Once you have downloaded SPM we need to tell matlab where it is located on your computer. This is done by adding the SPM folder into the matlab `path` (a set of folders where matlab will automatically look into when asked to run a specific function or program).

Type the following in the matlab command line and modify the `path_to_SPM` so that it matches the path of where you have unzipped SPM on your computer:
```matlab
addpath(path_to_SPM) %this will add SPM to the matlab path
```

If you don't want to do that every time you start matlab, you can just type:
```matlab
savepath %this saves the current state of the path for future sessions
```

Start SPM by typing this in the matlab command line:
```matlab
spm % starts the SPM (the graphic interface by default)
```
