# Acadgild_Assignment-4.3
Problem Statement
1. states=rownames(USArrests)

• Get states names with ‘w’.
• Get states names with ‘W’.

2. Prepare a histogram of the number of characters in each US state.

1. Answer:states=rownames(USArrests)
> states
 [1] "Alabama"        "Alaska"         "Arizona"        "Arkansas"       "California"    
 [6] "Colorado"       "Connecticut"    "Delaware"       "Florida"        "Georgia"       
[11] "Hawaii"         "Idaho"          "Illinois"       "Indiana"        "Iowa"          
[16] "Kansas"         "Kentucky"       "Louisiana"      "Maine"          "Maryland"      
[21] "Massachusetts"  "Michigan"       "Minnesota"      "Mississippi"    "Missouri"      
[26] "Montana"        "Nebraska"       "Nevada"         "New Hampshire"  "New Jersey"    
[31] "New Mexico"     "New York"       "North Carolina" "North Dakota"   "Ohio"          
[36] "Oklahoma"       "Oregon"         "Pennsylvania"   "Rhode Island"   "South Carolina"
[41] "South Dakota"   "Tennessee"      "Texas"          "Utah"           "Vermont"       
[46] "Virginia"       "Washington"     "West Virginia"  "Wisconsin"      "Wyoming"       
> states[grep("w",states)]
[1] "Delaware"      "Hawaii"        "Iowa"          "New Hampshire" "New Jersey"    "New Mexico"   
[7] "New York"     
> states[grep("W",states)]
[1] "Washington"    "West Virginia" "Wisconsin"     "Wyoming"

2. Answer: x<-nchar(states)
> x<-nchar(states)
> x
 [1]  7  6  7  8 10  8 11  8  7  7  6  5  8  7  4  6  8  9  5  8 13  8  9 11  8  7  8  6 13 10 10  8
[33] 14 12  4  8  6 12 12 14 12  9  5  4  7  8 10 13  9  7
> hist(x)
