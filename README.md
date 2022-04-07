# Shiny_Fish_Manager
Filter your dataset and automatically calculate catch per unit effort, relative weight, and proportional stock density of various freshwater sport fish species 

# Getting Started
- download the example dataset ("example_data.csv")
- install necessary packages into R 
- run app > choose the downloaded example dataset to load into the app 

# Limitations
- To use this application on your own data, your data must match the example dataframe names for 3 columns: waterbody, transect_number (sample site, sample station etc.), and species 
        - Species codes should also match that of the 'FSA' package R package. 
- Wr and PSD calculations are limited to the species present in this dataset. More species can be added with the same structure of this code if they are included in the 'FSA' R package. 
        - To find minimum size lengths for PSD calculations, use psdVal()
        - To find weight equations for Wr calculations, use wsVal()
- All species options within a waterbody show when a single transect is selected, regardless of if not all species are present in that site. Species will show a check mark in the filter but will not appear in the calculation boxes if that species does not occur in the selected sites. 
- This application assumes no errors are in your data when calculating. Best to do quality-assurance on your data before using this.
        - ex. If the weight of an idividual was typed into the data as 14 instead of the true value of 74, this will alter the resulting relative weight value- potentially to an extreme level depending on the species 


# Updates to Come 
- Error messages initially observed when opening the app will be replaced with messages to the user instructing them to load the appropriate items into the app
- Secondary pages will be added to the app that explain the meaning behind these variables and how managers use this information to enact management strategies 
- 
