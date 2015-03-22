# CCDC Software #

Algorithm is not available online at the moment...

**Algorithm developed for Continuous Change Detection and Classification (CCDC) of land cover using all available Landsat data.**

**Please cite the following**

**[paper 1](http://www.sciencedirect.com/science/article/pii/S0034425712000387):
Zhu, Z. and Woodcock, C. E., Continuous monitoring of forest disturbance using all available Landsat imagery, Remote Sensing of Environment (2012), doi:10.1016/j.rse.2011.10.030.(paper for CCDC version 1.0.)**

**[paper 2](http://www.sciencedirect.com/science/article/pii/S0034425714000248):
Zhu, Z. and Woodcock, C. E., Continuous change detection and classification of land cover using all available Landsat data, Remote Sensing of Environment (2014), doi.org/10.1016/j.rse.2014.01.011.(paper for CCDC version 7.3.)**

This algorithm has been applied to many parts of the world and you can see all located where it has been applied at [here](https://github.com/bullocke/Landsat-Database/blob/master/PRmap.geojson).

You can download the PPT with GIF images that explain the CCDC algorithm at this [link](https://www.dropbox.com/s/w23by47zrtnvyd3/ccdc_ppt.pptx?dl=0).

Or you can download the video that explain the CCDC algorithm at this [link (mp4)](https://www.dropbox.com/s/z2ts2glufx1y705/ccdc_mp4.mp4?dl=0) or [link (wmv)](https://www.dropbox.com/s/usybqoc61aszx75/ccdc_wmv.wmv?dl=0).


Bellow are all the revisions made for CCDC since its first publication (1.0 version)

Revisions: $ Date: 11/10/2014 $ Copyright: Zhe Zhu

Version 12.13: More infromation in "category" (11/10/2014)

This version (12.13) is used for the third round of LCMS project.

Command: TrendSeasonalFit\_v12Plot(N\_row,N\_col,min=0.5,T\_cg=0.99,n\_times=3,conse=6,B\_detect=2:6)

Version 12.12: Fit for pixels where Fmask fails (11/09/2014)

Version 12.11: Bug fixed in num\_fc (11/09/2014)

Version 12.10: Better multietmporal cloud detection at the beginning (11/06/2014)

Version 12.9:  Detect change only for land pixel (water/snow speical case) (10/31/2014)

Version 12.8:  Speed up by reducing time for RMSE and model computing (10/17/2014)

Version 12.7:  mini rmse should be larger than 10% of the mean (10/13/2014)

Version 12.6:  Fit model again when there are a 33.3% more data (10/08/2014)

Version 12.5:  Use subset of bands (2-6) for detecting surface change (10/01/2014)

Version 12.4:  Only apply multitemporal cloud masking during model initialization (09/29/2014)

Version 12.3:  Use subset of bands (3-5) to balance change in different dimensions (09/01/2014)

This version (12.3) is used for the second round of LCMS project.

Command: TrendSeasonalFit\_v12Plot(N\_row,N\_col,min=0.99,T\_cg=2,n\_times=3,conse=5,B\_detect=3:6)

Version 12.2:  Bug fixed in model intialization (08/14/2014)

Version 12.1:  Use subset of bands (3-6) to avoid atmosphere influences (08/04/2014)

Version 12.0   Detecting change based on probability (07/19/2014)

Version 11.6:  No need to change folder name & faster in speed (by Christ Holden 06/06/2014)

Version 11.5:  Improved calculation of temporally adjusted RMSE (04/23/2014)

Version 11.4:  Revise "rec\_cg.category" to better seperate different fit processes (04/01/2014)

This version (11.4) is used for generating synthetic data for ACRE project and detecting change for LCMS project.

Command: TrendSeasonalFit\_v11Plot(N\_row,N\_col,min=1,T\_cg=2,n\_times=3,conse=6,B\_detect=1:6)

Version 11.3:  Add "rec\_cg.magnitude" as indicator of change magnitude (04/01/2014)

Version 11.2:  Change very simple fit with mean value for start and end of timeseries (04/01/2014)

Version 11.1:  Do not need metadata in the image folder to run CCDC (03/25/2014)

Version 11.0:  Use change vector magnitude as threshold for detecting change (03/25/2014)

Version 10.13: Use subset of bands (1-6) to avoid atmosphere influences (01/31/2014)

Version 10.12: More accurate number of days per year "num\_yrs" (01/30/2014)

Version 10.11: RMSE updates with time series fit (01/26/2014)

Version 10.10: Update temperature extreme in recent studies (01/16/2014)

Version 10.9:  Find break in max value in any of the band (01/08/2014)

Version 10.8:  Add very simple fit with median value for start and end of timeseries (10/21/2013)

This version (10.8) is used for generating synthetic data for the LCMS project.

Command: TrendSeasonalFit\_v10Plot('stack',N\_row,N\_col,mini=0.5,T\_cg=3,n\_times=3,conse=6,B\_detect=2:6)

Version 10.7:  Better multitemporal cloud detection (10/19/2013)

Version 10.6:  Add "Tmax\_cg" for last step noise removal (10/18/2013)

Version 10.5:  Use subset of bands (2-6) to avoid atmosphere influences (10/18/2013)

Version 10.4:  Let dynamic fitting for pixels at the beginning (09/23/2013)

Version 10.3:  Able to detect change at the verying beginning (09/06/2013)

Version 10.2:  Add mini years "mini\_yrs" in model intialization (09/03/2013)

Version 10.1:  Reduce time for calcuating "v\_dif" (09/02/2013)

Version 10.0:  Fit for beginning and end of the time series (08/31/2013)

Version 9.9:   Only fit more than 50% of Landat images overlap area (08/28/2013)

Version 9.8:   Force model fit for persistent snow pixels (08/27/2013)

Version 9.7:   Add "rec\_cg.category" as indicator of fitting procudure (08/20/2013)

> Add rec\_cg.change\_prob as indicator of change probability (08/20/2013)

> Add rec\_cg.num\_obs ad indicator of number of observations (08/20/2013)

Version 9.6:   Remove mininum rmse "mini" and minimum years "mini\_yrs" (08/16/2013)

Version 9.5:   Model gets more coefficients with more observations (08/16/2013)

Version 9.4:   Bug fixed in calculating temporally adjusted rmse (08/01/2013)

Version 9.3:   Fit curve again after one year (03/28/2013)

This version (9.3) is used for mapping land cover for the IDS project.

Command: TrendSeasonalFit\_v9Plot('stack',N\_row,N\_col,T\_cg=2,n\_times=3,conse=4)

Version 9.2:   Use "mini = T\_const/T\_cg" for small rmse cases (03/26/2013)

Version 9.1:   Remove out of range pixels before time series analysis (02/09/2013)

Version 9.0:   Using 8 coefficients and lasso fit (02/01/2013)

Version 8.4:   Use "max v\_slope" instead of "average v\_slope" (01/16/2013)

Version 8.3:   Start initialization when "time\_span" > 1 year (01/16/2013)

Version 8.2:   Bug fixed in not fitting models at the begining (01/16/2013)

Version 8.1:   Bug fixed in counting "i" and "i\_span"(01/13/2013)

Version 8.0:   Temporally changing RMSE (01/09/2013)

Version 7.3:   Continuous Change Detection and Classification (CCDC) (07/11/2012)

This version (7.3) is explained by Zhu, Z. & Woodcock, C.E., Continuous Change Detection and Classification (CCDC) of land cover using all available Landsat data, Remote Sensing of Environment (2014).

Command: TrendSeasonalFit\_v7Plot('stack',N\_row,N\_col,T\_cg=3,n\_times=3,conse=3)

Version 1.0:   Continous Monitoring of Forest Disturbance Algorithm (CMFDA) (07/13/2010)

This version (1.0) is explained by Zhu, Z., Woodcock, C.E., Olofsson, P., Continuous monitoring of forest disturbance using all available Landsat data, Remote Sensing of Environment (2012).