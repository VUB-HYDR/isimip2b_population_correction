**Problem highlighted by Inne Vanderkelen (inne.vanderkelen@vub.be) and Wim Thiery (wim.thiery@vub.be)**
**Solution proposed by Ioan Sabin Taranu (sabin.taranu@vub.be)**

# Brief description of problem:
At the transition between population_histsoc_0p5deg_annual_1861-2005.nc4 and population_ssp2soc_0p5deg_annual_2006-2100.nc4 datasets (input datasets in the ISIMIP2b protocol) some spatial inconsistency is detected between individual gridcells. This issue may limit these data usability for analysis which is performed at gridcell level and is population dependent. Some figures representing these inconsistencies can be seen in: population_issues_ISIMIP2b_inputdata.pdf.

# Solution:
To overcome this issue, we propose a simple and well documented script (../scripts/population_data_correction_for_consistent_spatial_distribution_of_national_population.ipynb).
In addition to the correction algorithm, the provided jupyter notebook allow to execute a list of validation tests notifying the user of potential issues and plot some validation figures.

While we used this solution to correct only the population_ssp2soc_0p5deg_annual_2006-2100.nc4 dataset, it can be easily used to correct any other dataset suffering from the same problem of spatial inconsistency at the transition between datasets. On a regular computer, the entire correction procedure will take between 10-15 minutes for 100 years of global data at 0.5x0.5deg resolution. 

Due to potential copyrights issues, we do not provide any copy of the actual or corrected population data.
Therefore if the user wants to test the script, he/she will be required to download his own data from the ISIMIP official repository.

For any questions and support if needed, the user is invited to contact sabin.taranu@vub.be.

Best regards,
Sabin

22 November 2022