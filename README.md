# Remote-Kinetic-Energy-Advection-as-a-Predictor-of-Wind-Power-Extremes-over-India
 The framework establishes a physically grounded pathway linking large-scale kinetic energy transport to wind power reliability under climate variability and change.

 <img width="1401" height="1072" alt="framewrk" src="https://github.com/user-attachments/assets/9961e122-b9da-41db-8b3d-0435f9576894" />

Fig. Schematic of the methodological framework outlining the workflow from ERA5 wind
and geopotential data to Kinetic Energy (KE) fields, EOF-based dimensionality reduction, and
regression modeling. The left branch represents intra-seasonal MW variability modeled using Ridge
Regression, and the right branch illustrates interannual TWh variability modeled using Elastic Net
and Multinomial Logistic Regression on Meta-EOFs. 

<img width="1083" height="359" alt="eof1" src="https://github.com/user-attachments/assets/970fe7b9-c0e5-4884-a317-d93a0500674a" />

Fig. EOF spatial pattern and PC time series for KE generation data over the Indian
subcontinent. X is the data matrix, ϕ1 the eigenvector explaining the largest variance fraction, and
z1 the projection of X onto the ϕ1 basis.

<img width="2489" height="690" alt="nn1" src="https://github.com/user-attachments/assets/fa52ea7f-7e10-401c-bef4-dc87e8f9581e" />

Modeling intraseasonal variability of wind power generation during the 2017 (drought)
monsoon. Daily observed (red dotted) and modeled (blue: dominant KE advection, green: dom-
inant KE generation) power generation using ridge regression with the top 10 lag-adjusted principal
components (PCs) from each field. The model attains R² = 0.9, MSE = 0.01. Power generation
values are normalized for visualization.The right panel ranks the 10 most significant KE Adv and
KE Gen modes by contribution.

<img width="4623" height="605" alt="gy" src="https://github.com/user-attachments/assets/4845f37f-9cc7-4eed-b06f-f61acf372476" />

Spatial Empirical Orthogonal Function (EOF) patterns of the
top contributing modes, showing dominant intraseasonal structures of KE advection and generation
linked to intraseasonal variations.



