# Malagon-Vina-Anxiety2022

This repository contains the pre-processed data for the eLife publication Malagon-Vina et al:  https://doi.org/10.7554/eLife.83012

Manuscript_data.mat has several files with the pre-processed raw data.
 
There are two types of data. One belongs to the EPM (elevated plus maze), and the other to the ELM (elevated linear maze).
 
EPM files
 
All_E2N
All_E2S
All_W2N
All_W2S
Max_Center_E2N
Max_Center_E2S
Max_Center_W2N
Max_Center_W2S
BehaviouralReadsEPM
 
ELM files
All the rest.
 
Explanation of each file
 
EPM files
 
They are coded All_A2B, where A and B are two of the four possible arms in an EPM. So, for example, All_E2N is the data for the trajectory from East to North (W and S would be west and south). Each row is the Gaussian filtered place map for that specific trajectory. Max_Center_A2B variable is the spatial bin where the animals enter the centre.
 
The BehaviouralReadsEPM has three variables.
NumberT = Number of journeys during each recorded session
NumberTperMinute = same but normalised per minute
TimeSpent = calculations of the time spent in open arms, closed arms and centre.
 
ELM files
 
There are three types of files.
 
AllPlaceMapsXX contains all the place maps for a given configuration (CC, CO, CT and CCT, which is CC2 in the manuscript). The complete placemaps (raw firing rate and Gaussian), and the separated ones per direction of the journey (Coming and Going towards the changing arm). Each row is a recorded neuron, and the columns are spatial bins. The variable centres define the spatial bin, considered the maze's centre. If an R precedes the name (e.g. RAllPlaceMapsXX) those are the maps created with the residuals of the firing vs speed regressions.
 
AllSparsityXX is the same as the previous one, but only the sparsity calculations per neuron.
 
Maps_TbT_XX is the same naming convention as the previous files. This file contains the trial by trial (in this case, each journey towards the changing arm) for each neuron in their given session. Column 1 has the firing rate matrix (rows are the trials, and columns are the spatial bins), and Column 2 is the spatial bin for the centre.
 
BehaviouralReads_XX has the same naming convention. It has the time spent on each arm, plus the speed. All the arms are divided into Open and Close. Close is the part of the ELM that never changes, while open is the one that changes (sometimes open, sometimes texture), depending on the configuration XX.

Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
