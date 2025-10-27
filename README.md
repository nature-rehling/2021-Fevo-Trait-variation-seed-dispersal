################################################################################
################################################################################

This package contains data from:

################################################################################

Rehling, F., Jaroszewicz, B., Braasch, L.B., Albrecht, J., Jordano, P., Schlautmann, J., Farwig, N., Schabo, D. G. (2021):
Within-species trait variation can lead to size limitations in seed dispersal of small-fruited plants

Corresponding author - today: Rehling, Finn; University of Freiburg
Email: finn.rehling@nature.uni-freiburg.de

################################################################################

The package contains four data files (each in .csv and .xlsx format) that were used in the analyses of the above mentioned publication.
The R script "Sizelimitations_R" is in .txt format, including the analyses of Rehling et al. (2021).

The structures of the data files are listed below with detailed descriptions of their contents.

################################################################################

Structure and description of data files that were used in the main analyses

################################################################################

1. overview_size
Mean fruit diameter of fleshy-fruited plants and mean gape width of seed-dispersing animals in Bialowieza forest (Poland)
'data.frame':	45 obs. of  3 variables:
 $ species: character, taxonomic species names of plants and animals
 $ size   : numeric, unit in [cm*100]
 $ class  : levels, taxonomic class, "plants" or "animals"

2. maxmeanfruit
'data.frame':	30 obs. of  5 variables:
 $ species  : character, taxonomic species names of the animals
 $ number   : integer, number of replicates (independent visits on fruiting plants)
 $ maxfruit : numeric, fruit diameter of largest consumed fruits, unit in [cm*100], based on Albrecht et al. 2013 and Schlautmann et al. 2021
 $ meanfruit: numeric, mean fruit diameter of consumed fruits, unit in [cm*100], based on only Albrecht et al. 2013
 $ gape     : numeric, gape width, unit in [cm*100]

3. divers_disp
Binary interaction matrix between plants and their dispersers
'data.frame':	15 obs. of  41 variables:
 $ plants    : character, taxonomic species names of the plant species
 $ f.diameter: numeric, fruit diameter, unit in [cm*100]
 $ Apfl      : integer, interactions with "Apodemus flavicollis", yes (1), no (2)
 $ Bobo      : integer, interactions with "Bos bonasus", yes (1), no (2)
 $ Caer      : integer, interactions with "Carpodacus erythrinus", yes (1), no (2)
 $ Ceel      : integer, interactions with "Cervus elaphus", yes (1), no (2)
 $ Coco      : integer, interactions with "Coccothraustes coccothraustes", yes (1), no (2)
 $ Cola      : integer, interactions with "Columbus palumbus", yes (1), no (2)
 $ Dele      : integer, interactions with "Dendrocopos leucotos", yes (1), no (2)
 $ Dema      : integer, interactions with "Dendrocopos major", yes (1), no (2)
 $ Deme      : integer, interactions with "Dendrocopos medius", yes (1), no (2)
 $ Drma      : integer, interactions with "Dryocopus martius", yes (1), no (2)
 $ Drni      : integer, interactions with "Dryomys nitedula", yes (1), no (2)
 $ Erru      : integer, interactions with "Ficedula hypoleuca", yes (1), no (2)
 $ Fihy      : integer, interactions with "Ficedula parva", yes (1), no (2)
 $ Fipa      : integer, interactions with "Fringilla coelebs", yes (1), no (2)
 $ Gagl      : integer, interactions with "Garrulus glandarius", yes (1), no (2)
 $ Hiic      : integer, interactions with "Hippolais icterina", yes (1), no (2)
 $ Lulu      : integer, interactions with "Luscinia luscinia", yes (1), no (2)
 $ Mama      : integer, interactions with "Martes martes", yes (1), no (2)
 $ Muav      : integer, interactions with "Muscardinus avellanarius", yes (1), no (2)
 $ Must      : integer, interactions with "Muscicapa striata", yes (1), no (2)
 $ Mygl      : integer, interactions with "Myodes glareolus", yes (1), no (2)
 $ Oror      : integer, interactions with "Oriolus oriolus", yes (1), no (2)
 $ Pama      : integer, interactions with "Parus major", yes (1), no (2)
 $ Phtr      : integer, interactions with "Phylloscopus trochilus", yes (1), no (2)
 $ Popa      : integer, interactions with "Poecile palustris", yes (1), no (2)
 $ Prmo      : integer, interactions with "Prunella modularis", yes (1), no (2)
 $ Pypy      : integer, interactions with "Pyrrhula pyrrhula", yes (1), no (2)
 $ Scvu      : integer, interactions with "Sciurus vulgaris", yes (1), no (2)
 $ Sieu      : integer, interactions with "Sitta europaea", yes (1), no (2)
 $ Syat      : integer, interactions with "Sylvia atricapilla", yes (1), no (2)
 $ Sybo      : integer, interactions with "Sylvia borin", yes (1), no (2)
 $ Tebo      : integer, interactions with "Tetrastes bonasia", yes (1), no (2)
 $ Tuil      : integer, interactions with "Turdus iliacus", yes (1), no (2)
 $ Tume      : integer, interactions with "Turdus merula", yes (1), no (2)
 $ Tuph      : integer, interactions with "Turdus philomelos", yes (1), no (2)
 $ Tupi      : integer, interactions with "Turdus pilaris", yes (1), no (2)
 $ Tuvi      : integer, interactions with "Turdus viscivorus", yes (1), no (2)
 $ diversity : integer, number of interacting disperser species, i.e. plant perspective

4. fruitseeddata
'data.frame':	1012 obs. of  10 variables:
 $ plant     : Factor, taxonomic species names of the nine most abundant plant species in the study
 $ f.mass    : integer, mass of single fruit, unit in [mg]
 $ f.size1   : numeric, length of fruits, unit in [mm]
 $ f.size2   : numeric, width of fruits, unit in [mm] 
 $ no.seeds  : integer, number of seeds per fruit
 $ parent    : factor, parent name nested in plant species
 $ parentname: character, unique parent name
 $ t.seeds   : numeric, total mass of seeds per fruit, unit in [mg]
 $ forest    : factor, forest type, "managed" or "old-growth"
 $ pred      : integer, pre-dispersal seed predation in S. aucuparia, (1) yes, (0) no
