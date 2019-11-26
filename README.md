Join our [slack workspace](https://join.slack.com/t/fmriworkshopuclouvain/shared_invite/enQtODQ3NTc3NjkwMTUwLWJmZDQzN2ZmZjdlNmU2NTBjNDFhODUwMzg5ODUxNGNjNzI4YjlmMTcwYzY4M2VhYTQzZGRmOTFhMWZjMjFlZmE) to keep in touch and exchange information quickly with all the participants.

___

**IMPORTANT: The workshop will start at 8H30 every day.**
___


<!-- TOC -->

- [UCLouvain fMRI workshop - november 2019](#uclouvain-fmri-workshop---november-2019)
  - [PRELIMINARY PROGRAM](#preliminary-program)
    - [Day1: November 27th](#day1-november-27th)
      - [Morning: Jorge Jovicich](#morning-jorge-jovicich)
      - [Afternoon: Jorge Jovicich](#afternoon-jorge-jovicich)
      - [Evening: get together for a drink](#evening-get-together-for-a-drink)
    - [Day 2: November 28th](#day-2-november-28th)
      - [Morning: Christophe Phillips](#morning-christophe-phillips)
      - [Afternoon: Hans Op de Beeck](#afternoon-hans-op-de-beeck)
    - [Day 3: November 29th](#day-3-november-29th)
      - [Morning and afternoon: Mohamed + Remi + Olivier](#morning-and-afternoon-mohamed--remi--olivier)
  - [Practical information](#practical-information)
    - [What you will need](#what-you-will-need)
    - [Installing SPM12](#installing-spm12)

<!-- /TOC -->


# UCLouvain fMRI workshop - november 2019

In the context of an ISPY-funded stay at UCLouvain of Jorge Jovicich, director of the MRI lab at CIMeC-IT, we will organise an (f)MRI workshop November 27 to 29, 2019.

Additional speakers in the workshop will be
- Christophe Phillips (Ulg)
- Hans Op de Beeck (KUL)
- Mohamed Rezk (UCLouvain),
- Remi Gau (UCLouvain)
- Olivier Collignon (UCLouvain)

Phd students registered in an FNRS doctoral school will surely be able to credit this training activity.

The workshop targets beginners and aim to explain the basic principles of (f)MRI recording and analyses. So no previous knowledge is required. Intermediate/advanced neuroimagers may surely find it useful to refresh or consolidate their knowledge but the workshop is not designed to cover the latest methodological trends.

Aside the formal "teaching", we will try to have moments for informal discussions with the speakers during breaks, including having a drink at the end of the day in a bar nearby (make sure to add this in the agenda).

The workshop will be free of charge for anyone attending and will be held in English.


##  PRELIMINARY PROGRAM

The first 2 days are mostly "theoretical" and the last day is more "practical" (including hands-on). Due to practical constraints, this last day is limited to max. 50 people. If more than 50 people are interested, priority will be given to early Phd students.

___
### Day1: November 27th

**Location:** Auditoire Central J. MAISIN (max. 120 persons), Rue Emmanuelle Mounier 51, 1200 Brussels (Wolluwé) ([google map](https://goo.gl/maps/kv6Sxp86fmr6PEYv8) ; [pdf](./map_wolluwe.pdf))


#### Morning: Jorge Jovicich

**Start at 8H30**

-   Basics: NMR signal, generating an MRI, MRI contrast

-   Pause: 10H30 - 11H00

-   Structural MRI: Contrasts for morphometry. Challenges

-   Lunch: 12H30 - 14H00

#### Afternoon: Jorge Jovicich

-   Functional MRI: BOLD contrast. Fast MRI. Preprocessing. Challenges

-   Pause: 15H30 - 16H00

-   Diffusion MRI: Diffusion contrast. Preprocessing. Tractography. Challenges

#### Evening: get together for a drink

___
### Day 2: November 28th

**Start at 8H30**

**Location:** Auditoire Central J. MAISIN (max. 120 persons), Rue Emmanuelle Mounier 51, 1200 Brussels (Wolluwé) ([google map](https://goo.gl/maps/kv6Sxp86fmr6PEYv8) ; [pdf](./map_wolluwe.pdf))


#### Morning: Christophe Phillips

-   GLM principle & 1st level fMRI model, aka. FFX
-   Contrasts & Classical Inference
-   Group analysis, aka. RFX

-   Pause: 10H30 - 11H00

-   Mulitple Comparison & Image-wise inference
-   Functional and effective connectivity (eg PPI, DCM)- if times allow.

-   Lunch: 12H30 - 14H00

#### Afternoon: Hans Op de Beeck

-   Multivariate analyses: History, principles, advantages....
-   Multivariate analyses: The methods (Correlation, Decoding, RSA....)

-   Pause: 15H30 - 16H00

-   Multivariate connectivity

___
### Day 3: November 29th

**Start at 8H30**

**Location:** Salle Shannon - Maxwell Building - Place du Levant, 3, Louvain-la-Neuve  ([google map](https://goo.gl/maps/UYkweqZo7QsLxbyWA))


#### Morning and afternoon: Mohamed + Remi + Olivier

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
