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

## Theory

The first 2 days are mostly "theoretical" and will take place at Auditoire Central J. MAISIN (max. 120 persons), Rue Emmanuelle Mounier 51, 1200 Brussels (Wolluwé).

## Practice

The last day is more "practical" (including hands-on) and will take place at Salle Shannon - Maxwell Building - Place du Levant, 3, Louvain-la-Neuve.

Due to practical constraints, this last day is limited to max. 50 people. If more than 50 people are interested, priority will be given to early Phd students.

For the practical, it is mandatory that you come with your own laptop and have the following things on it:

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

### Add SPM to the matlab path
Type the following in the matlab command line and modify the `path_to_SPM` so that it matches the path of where you have unzipped SPM on your computer:
```matlab
addpath(path_to_SPM)
```

Start SPM by typing this in the matlab command line:
```matlab
spm fmri
```


##  PRELIMINARY PROGRAM


### Day1: November 27th

**Location:** Auditoire Central J. MAISIN (max. 120 persons), Rue Emmanuelle Mounier 51, 1200 Brussels (Wolluwé)

#### Morning: Jorge Jovicich

-   Basics: NMR signal, generating an MRI, MRI contrast
-   Structural MRI: Contrasts for morphometry. Challenges

#### Afternoon: Jorge Jovicich

-   Functional MRI: BOLD contrast. Fast MRI. Preprocessing. Challenges
-   Diffusion MRI: Diffusion contrast. Preprocessing. Tractography. Challenges


### Day 2: November 28th

**Location:** Auditoire Central J. MAISIN (max. 120 persons), Rue Emmanuelle Mounier 51, 1200 Brussels (Wolluwé)

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

**Location:** Salle Shannon - Maxwell Building - Place du Levant, 3, Louvain-la-Neuve

#### Morning and afternoon: Mohamed + Remi + Olivier

-   Experimental design
-   Illustration of the different methods with real data
-   BIDS format + Github (scripts)
-   Hands-on
