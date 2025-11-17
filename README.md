# Remote-Kinetic-Energy-Advection-as-a-Predictor-of-Wind-Power-Extremes-over-India
 The framework establishes a physically grounded pathway linking large-scale kinetic energy transport to wind power reliability under climate variability and change.

 <img width="1710" height="654" alt="ke" src="https://github.com/user-attachments/assets/45784915-c8d7-475b-b751-28c6c741ce72" />

Fig 1. Spatial patterns of (left) conversion of Available Potential Energy (APE) to Kinetic Energy
(KE) and (right) horizontal KE advection outflow in red during August 2017, the month of peak
wind power generation. Blue shading in left indicates regions of strong APE–KE conversion, and red
shading in right denotes strong KE outflow. Black markers show major wind farm locations across
India. These fields illustrate the large-scale pathways feeding wind power production over India.


 <img width="1401" height="1072" alt="framewrk" src="https://github.com/user-attachments/assets/9961e122-b9da-41db-8b3d-0435f9576894" />

Fig 2. Schematic of the methodological framework outlining the workflow from ERA5 wind
and geopotential data to Kinetic Energy (KE) fields, EOF-based dimensionality reduction, and
regression modeling. The left branch represents intra-seasonal MW variability modeled using Ridge
Regression, and the right branch illustrates interannual TWh variability modeled using Elastic Net
and Multinomial Logistic Regression on Meta-EOFs. 

<img width="1083" height="359" alt="eof1" src="https://github.com/user-attachments/assets/970fe7b9-c0e5-4884-a317-d93a0500674a" />

Fig 3. EOF spatial pattern and PC time series for KE generation data over the Indian
subcontinent. X is the data matrix, ϕ1 the eigenvector explaining the largest variance fraction, and
z1 the projection of X onto the ϕ1 basis.

## Intra-seasonal MW modeling

<img width="2489" height="690" alt="nn1" src="https://github.com/user-attachments/assets/fa52ea7f-7e10-401c-bef4-dc87e8f9581e" />

Fig 4. Modeling intraseasonal variability of wind power generation during the 2017 (drought)
monsoon. Daily observed (red dotted) and modeled (blue: dominant KE advection, green: dom-
inant KE generation) power generation using ridge regression with the top 10 lag-adjusted principal
components (PCs) from each field. The model attains R² = 0.9, MSE = 0.01. Power generation
values are normalized for visualization.The right panel ranks the 10 most significant KE Adv and
KE Gen modes by contribution.

<img width="4623" height="605" alt="gy" src="https://github.com/user-attachments/assets/4845f37f-9cc7-4eed-b06f-f61acf372476" />

Fig 5. Spatial Empirical Orthogonal Function (EOF) patterns of the
top contributing modes, showing dominant intraseasonal structures of KE advection and generation
linked to intraseasonal variations.

### Summary

This anlysis illustrates the model performance for the drought year 2017. The
ridge-regression model is trained on the top ten lag-adjusted principal components
(PCs), as measured by variance explained, from KE advection and generation. The
model captures the observed intraseasonal variability with strong agreement between
observed and modeled power generation(R² = 0.9, MSE = 0.01). The right-hand
panel ranks the contributions of each predictor (PC1–PC10 from KEadv; PC11–PC20
from KEgen), highlighting that KEadv PC1 and PC7 dominate predictability.


<img width="629" height="389" alt="image" src="https://github.com/user-attachments/assets/d9aff4c5-4299-4db7-8b63-f2bdb4c66130" />


## Interannual TWh modeling

<img width="2000" height="2500" alt="energy_twh" src="https://github.com/user-attachments/assets/246ea6c9-bc3b-4eb3-b5d2-a61842a59beb" />

Fig 6. Seasonal total generation (TWh) for each year as Area Under Curve(AUC) of power generation time series during monsoon season.(DOY: Day Of the Year)

<img width="2090" height="690" alt="gt" src="https://github.com/user-attachments/assets/a1df308f-18b7-4d34-9ff9-8525bab604c8" />

Fig 7. (Left) Coefficient of determination (R²) between individual PCs of KE advection and gener-
ation and seasonal TWh, showing the dominant predictive power of the first KE Adv mode. (Right)
Correlation between standardized EOF1 variances for KE Adv and KE Gen(R²=0.63), demonstrat-
ing coherent interannual modulation by large-scale kinetic-energy generation and fluxes of national
wind power output. Overall, KE Adv PC1 remains a more reliable predictor of TWh across years.

<img width="2252" height="636" alt="huo" src="https://github.com/user-attachments/assets/e97df544-33d7-4388-881f-b6fd33fcbdf6" />

Fig 8. patial structures of the top Meta-EOFs, highlighting key
regions of high variability in kinetic-energy advection that underpin predictability of annual wind
power generation.

<img width="1801" height="766" alt="p" src="https://github.com/user-attachments/assets/7e06e17d-fc47-498e-b9a2-97c2b18bf61b" />

Fig 9. Elastic-Net regression of annual TWh using the top five Meta-EOFs (EOFs of annual
EOF1 patterns). Negative residuals correspond to wind-drought years (red) and positive residuals
to flood years (blue). The model achieves R² = 0.75, RMSE = 2.41 TWh. Right panel shows ranked
contributions of the Meta-EOFs. 

<img width="2566" height="924" alt="hu" src="https://github.com/user-attachments/assets/c4de4ab8-2f80-4e5b-b6bb-5095d068c1fe" />

Fig 10. Multinomial logistic-regression (MLR) classification of drought, normal, and flood years
using Meta-EOF predictors. (Left) Model coefficients indicate the direction and magnitude of each
Meta-EOF’s influence on class probability. (Right) Permutation importance per class quantifies the
contribution of each Meta-EOF phase to correct classification, emphasizing physically interpretable
large-scale KE-transport patterns associated with each category.

### Summary

This analysis demonstrates that among all predictors, Meta-EOF1, Meta-EOF3,
and Meta-EOF8 exert the strongest influence on year-type classification.
Meta-EOF1 captures the strength of cross-equatorial flow into the Arabian Sea,
Meta-EOF3 represents basin-wide rotational anomalies, and Meta-EOF8 reflects
regional circulation adjustments over peninsular India. Drought years correspond to
the negative phase of these modes, while flood years correspond to positive phases.
Because these modes recur and evolve on seasonal lead times, they offer a physically
grounded basis for early-warning indicators of national wind-generation anomalies.








