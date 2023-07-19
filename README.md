## MonarchOE_Temperature_Infection2019
A 2019 experiment testing Monarch-OE performance and infection outcomes across a gradient of five constant temperatures.

Authors: Isabella G. Ragonese, Maya R. Sarkar, Richard J. Hall, and Sonia Altizer

Funding:
This work was supported by the National Science Foundation [Graduate Research Fellowship and Research Traineeship DGE-1545433 to I.G.R.; DEB-1754392 to S.A. and R.J.H.] in conjunction with the University of Georgia through the Population Biology of Infectious Diseases REU Site [DBI-1156707]. The funders had no role in study design, data collection and analysis

Research Facility: University of Georgia

Keywords: Danaus plexippus; Ophryocystis elektroscirrha; extreme heat; temperature; infection

Methods: We used a constant temperature experiment to explore how temperature influences components of host and parasite performance in monarch butterflies (Danaus plexippus) and their protozoan parasite OE (Ophryocystis elektroscirrha). Using five constant temperature treatments spanning 18-34°C, we measured monarch development, survival, size, immune function, and OE infection status and intensity. Below, datasheet columns are defined. Analyses were completed in R.

### Metadata for 2019 Temperature-Infection experiment

File: mtemp_comp_Nov1_2021.csv (comprehensive data for majority of analysis)
"ID" = uniquie monarch identification number (1-450)               
"Temp" = Temperature treamtment (18, 22, 26, 30, 34)            
"Lineage" = One of three outbred host lineages (B, D, F)          
"OE_strain" = Parasite treatment (control, E3-less virulent or E10-more virulent)       
"Inoculation" = date fed inoculation leaf (all monarchs were inoculated outside of incubators - except for a few that took         multiple days to consume the leaf (mostly in the coldest treatments; only ~3 for 34C))    
"Into_pint" = date put into an individual pint within the incubator       
"Bleed_stage.x" = assigned stage to be sampled for hemolymph (None, Larva, Pupa) (from master datasheet)  
"Bleed_date.x" = date hemolymph taken (from master datasheet)     
"Death_date" = date died (most entries have notes on stage at death)      
"Pupation_date" = date pupated (either as J splitting skin or completed pupa)  
"Eclosion_date" = date adult emerged   
"Surv_pupa" = binary survival to pupal stage (1,0)       
"Surv_adult" = binary survival to adult stage (1,0)       
"Wing_deformity" = score of how deformed wings are (0 = no deformity to 3 = extremely deformed)  
"Adult_death_date" = date of adult death
"Sex" = Male or female (for all individuals surviving to adulthood)              
"Infection_status" = binary infected or not (1,0) 
"OE_score" = infection intensity from tape samples (0 to 5)       
"Dev_pupa" = time to pupation (days)        
"Dev_adult" = time to adult emergence (days)       
"Adult_longevity" = lifespan as an adult (death - emergence)(days)  
"NOTES" = any notes on individual during experiment           
"Bleed_date.y" = date hemolymph taken (from hemolymph datasheet)     
"Who" = researcher who counted hemocytes             
"Bleed_stage.y" = stage actually sampled for hemolymph (None, Larva, Pupa) (from hemocyte datasheet)    
"Mass" = mass of some larvae and pupa (only for subset of bled individuals) (g, from hemocyte datasheet)            
"AvgHemo" = average number of hemocytes in one chamber of kova slide (from hemocyte datasheet)          
"Hemo_ul" = hemocytes per microliter (AvgHemo*10) (+1 so that log10 works) (from hemocyte datasheet) 
"LogHemo" = Log base 10 of Hemo_ul (from hemocyte datasheet)        
"PropPlasm" = proportion of hemocytes that were classified as plasmatocytes (out of first ~100 cells in kova chambers (or          all cells in kova chambers if <100) (from hemocyte datasheet)      
"PropOeno" = proportion of hemocytes that were classified as oenocytoids (out of first ~100 cells in kova chambers (or all         cells in kova chambers if <100) (from hemocyte datasheet)           
"PropSpher" = proportion of hemocytes that were classified as spheroids (out of first ~100 cells in kova chambers (or all         cells in kova chambers if <100)(from hemocyte datasheet) 
"PropGran" = proportion of hemocytes that were classified as granulocytes (out of first ~100 cells in kova chambers (or all         cells in kova chambers if <100)(from hemocyte datasheet) 
"Initials" = researcher who counted vortexing slides for spore load        
"Date" = date sample vortexed            
"AvgOE_count" =  average number of OE spores in one chamber of kova slide    
"Spore_load" =  OE spores per monarch (AvgOE_count*10 (OE per ul) and * 5000 as monarchs were vortexed in 5mL of water) (+1         so that log10 works)  
"logSpore_load" = Log base 10 of Spore_load
"Area" = Wing area in mm^2
"Length" = Wing length in mm
"Breadth" = Wing width in mm
"AspectRatio" = Wing length / breadth (measure of wing elongation - migratory wings typically more elongated)
"FinalAbsorbance" = Phenoloxidase assay absorbance value at the final timestep (from BioTek microplate reader software)

File: Hemocyte_counts_June5.csv (hemocyte counts and concentration)
See comprehensive datasheet, includes raw count values for hemocytometer chambers plus counts of immune cell types


File: Merozoites_7_21.csv (file with internal parasite counts)
"ID" = uniquie monarch identification number (of those bled at the pupal stage)
"Date Bled" = date hemolymph taken
"Mass (g)" = pupal mass
"AvgOE" = average merozoites in one chamber of kova slide
"OE_ul" = merozoites per microliter (AvgHemo*10)
"LogOE" = Log base ten of ("OE_ul" + 1)
"Notes" = notes on the quality of the hemolymph sample and the stages of OE observed

