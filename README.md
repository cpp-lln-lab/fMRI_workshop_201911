Join our [slack workspace](https://join.slack.com/t/fmriworkshopuclouvain/shared_invite/enQtODQ3NTc3NjkwMTUwLWJmZDQzN2ZmZjdlNmU2NTBjNDFhODUwMzg5ODUxNGNjNzI4YjlmMTcwYzY4M2VhYTQzZGRmOTFhMWZjMjFlZmE) to keep in touch and exchange information quickly with all the participants.

___

**IMPORTANT: The workshop will start at 8H30 every day.**
___

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


### Day1: November 27th

**Location:** Auditoire Central J. MAISIN (max. 120 persons), Rue Emmanuelle Mounier 51, 1200 Brussels (Wolluwé) ([google map](https://goo.gl/maps/kv6Sxp86fmr6PEYv8) ; [pdf](./map_wolluwe.pdf))

#### Morning: Jorge Jovicich

-   Basics: NMR signal, generating an MRI, MRI contrast
-   Structural MRI: Contrasts for morphometry. Challenges

#### Afternoon: Jorge Jovicich

-   Functional MRI: BOLD contrast. Fast MRI. Preprocessing. Challenges
-   Diffusion MRI: Diffusion contrast. Preprocessing. Tractography. Challenges


### Day 2: November 28th

**Location:** Auditoire Central J. MAISIN (max. 120 persons), Rue Emmanuelle Mounier 51, 1200 Brussels (Wolluwé) ([google map](https://goo.gl/maps/kv6Sxp86fmr6PEYv8) ; [pdf](./map_wolluwe.pdf))

#### Morning: Christophe Phillips

-   GLM principle & 1st level fMRI model, aka. FFX
-   Contrasts & Classical Inference
-   Group analysis, aka. RFX
-   Mulitple Comparison & Image-wise inference
-   Functional and effective connectivity (eg PPI, DCM)- if times allow.

#### Afternoon: Hans Op de Beeck

-   Multivariate analyses: History, principles, advantages....
-   Multivariate analyses: The methods (Correlation, Decoding, RSA....)
-   Multivariate connectivity


### Day 3: November 29th

**Location:** Salle Shannon - Maxwell Building - Place du Levant, 3, Louvain-la-Neuve  ([google map](https://goo.gl/maps/UYkweqZo7QsLxbyWA))

#### Morning and afternoon: Mohamed + Remi + Olivier

-   Experimental design
-   Illustration of the different methods with real data
-   BIDS format + Github (scripts)
-   Hands-on


## Practical information


### What you will need

For the hands-on part, it is mandatory that you come with your own laptop and have the following things on it:

-   5 gigabytes of free space to comfortably run the analysis
-   Matlab
-   [Atom text editor](https://atom.io/)
-   [MRIcron](https://www.nitrc.org/projects/mricron/) and [MRIcroGL](https://www.nitrc.org/frs/?group_id=889) for the easy visualization of MRI images
-   [SPM12](https://www.fil.ion.ucl.ac.uk/spm/software/download/)
-   Code for the automated analysis pipeline [v0.0.1](https://github.com/cpp-lln-lab/CPP_BIDS_SPM_pipeline/releases/tag/v0.0.1)
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
