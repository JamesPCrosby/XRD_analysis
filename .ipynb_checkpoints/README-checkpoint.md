# XRD_analysis

# Code allows for the loading of either text or csv files, however this has to be writtin into the code yourself. Need to create a function that will allow for the recognition of file type and use the appropriate file loader

# Plotted input data using the matplotlib software.
# Removed any data points that were below zero.  This data points came about because of the noise in the machine. 

# Utilised a smoothing factor with python code itself.  This reduced the overall noise and aids for peak identification.
# Utilised peak finding procedure within the peakutils module.  This allows you to set the minimum amplitude of the peak.  The program then determines all y values that are above this value and their corresponding x values.  An issue with this is the noise means that only large peaks are able to be identified reliable.  Reducing the minimum amplitude for consideration results in multiple false peaks being identified.  This issue may need to looked at again to determine its worth.

# Multipeak_Fitting_Example

# Multipeak fitting has been attempted successfully on test data generated with the python environment.  However, this procedure looks promising, however you have to manually implement choose how many peaks within your data that you want to fit and what kind of peak you want to fit, e.g. Gaussian, Lorentzian etc.  This is fine for the ideal data as we know what kind of data is being fit as we are self generating it.  

# To fit the XRD data itself, I think we need to create a function that you either choose what kind of peaks that you want to fit and perform a R-squared or other statistical measurement to determine which fit is the best.  However, this would be a very labourious task if the data contains lots of peaks, where it is not clear what kind of peak will be needed to create the best fit.  

# I am hoping to create code that will either identify each peak or has some sort of user input for the number of peaks and their approximate location with the specta.  I would then try and implement a procedure where the code plots each peak with the three main peak types, Gaussian, Lorentzian and Voigt/PseudoVoigt and fits each peak with the peak that produces the least statiscal divergence.  

# This is the end goal of the software, however, this may be beyond my capabilities at present.

# JAMES CROSBY
