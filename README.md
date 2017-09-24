# Sound-Demo-Package
A Demo pipeline package for using DDWiener and SOUND

|| Introduction || 

The purpose of this package is to show through a practical MATLAB example how DDWiener and SOUND can be used to clean noisy EEG data. The MATLAB programs also show how a simple three-layer spherical head model, needed for SOUND, can be computed with the theoretical locations of the electrodes.

|| Terms of use ||

Copyright: 2017 Tuomas P. Mutanen, Johanna Metsomaa, Sara Liljander, and Risto J. Ilmoniemi

1. The provided Matlab demo package and/or the results can be used for a non-commercial or academic purpose only.
2. When the demo package is used to obtain new scientific results, the original article has to be cited.
3. When the user distributes a method, which depends on the demo package, the original article has to be cited with the mentioning of this Demo Package.
4. The Authors provide no support for using the demo package.  
5. The Demo package comes with no warranty: THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. (The CAPITALIZED text is from the MIT License.)



|| System requirements ||

The programs in this package are meant to be used on a standard desktop. The package has been tested with Windows 7 and Mac OS X 10.10.5. The programs in this package are written in MATLAB code and, therefore, require the MATLAB software to work. Prior to publishing, the package has been tested with MATLAB Releases R2015b and R2016b. The authors cannot guarantee that the programs will work with other MATLAB releases.
Within the package, you can find a program <MAIN_SCRIPT.m> that demonstrates how DDWiener and SOUND can be used alongside the open-source MATLAB toolbox EEGLAB (Delorme and Makeig, 2004) to clean a sample EEG dataset. The sample EEG dataset, used in the demo package, can be downloaded from the HeadIT Data Repository (available online http://headit.ucsd.edu/) maintained by the Swartz Center for Computational Neuroscience at the University of California at San Diego. The used dataset corresponds to the study of Auditory Two-Choice Response Task with an Ignored Feature Difference, session 7, recording 1 (available online http://headit.ucsd.edu/recording_sessions/99bc255c-a238-11e2-b5e7-0050563f2612). Note that you also need to download the .elp file containing the EEG-channel locations. In order to use the HeadIT Data Repository, the user must agree to the HeadIT Data Repository Terms of use and Data use agreement. For more details on the dataset, see the HeadIT Data Repository site.
Since the used sample EEG dataset is in Biosemi data format (.bdf), the BioSig toolbox (Schlögl and Brunner, 2008; available online http://biosig.sourceforge.net/download.html) is also needed. The provided demo package has been tested with EEGLAB toolbox Version 14.0.0b and BioSig toolbox Version 3.1.0. The authors cannot guarantee that the demo package will work as intended with other EEGLAB and BioSig versions.
The sample dataset has been measured with a 254-channel EEG system. Due to the large number of EEG electrodes, it is only likely that the data contain a few corrupted channels. Running the program <MAIN_SCRIPT.m> demonstrates how the corrupted   channels can be cleaned in a straightforward manner with minimal user interference. Because of the high dimensionality of the sample dataset, running the program can take several minutes. For more details on DDWiener and SOUND, see the original article by Mutanen et al. (in press).

|| Running the program ||

1. Download and install the EEGLAB toolbox (Version 14.0.0b has been tested; available online https://sccn.ucsd.edu/eeglab/downloadtoolbox.php).
2. Download and install the BioSig toolbox (Version 3.1.0 has been tested; available online http://biosig.sourceforge.net/download.html) in the EEGLAB “plugins” sub-folder.
3. Download the sample EEG dataset (eeg_recording_1.bdf) and the file containing the channel locations (channel_locations.elp) from the HeadIT Data Repository (available online http://headit.ucsd.edu/recording_sessions/99bc255c-a238-11e2-b5e7-0050563f2612).
4. Download and extract the SOUND demo package.
5. Make sure that all the needed folders and files (listed above) are located in your MATLAB path.
6. Open the program <MAIN_SCRIPT.m> in MATLAB. You can either run the whole script at once or run the different sections step by step. The sections have been numbered and are intended to be run in the specified order. The programs in the package are meant to be self-explanatory after reading the original article by Mutanen et al. (in revision). 

|| Contacts / Reporting bugs ||

	This demo package was built merely for demonstration purposes, and thus, should not be treated as a finished product. In a case you find any bugs or compatibility issues with certain operation systems or MATLAB/EEGLAB versions, you should inform them directly to Tuomas Mutanen or Johanna Metsomaa, by email: tuomas.mutanen@gmail.com or johanna.metsomaa@gmail.com, respectively. 

|| Acknowledgment ||

	This work was supported by the Academy of Finland, The Finnish Cultural Foundation, The Foundation for Aalto University Science and Technology, the Kymenlaakso Regional fund of the Finnish Cultural Foundation, and the Finnish Brain Foundation.
	Data used for developing and testing this demo package were downloaded from the HeadIT Data Repository (http://www.headit.org), supported by grants to the HeadIT (R01-MH084819) and EEGLAB (5-R01-NS047293-08) funded by the National Institutes of Health, U.S.A.” 	



References

Delorme, A., Makeig, S. 2004. EEGLAB: an open source toolbox for analysis of single-trial EEG dynamics including independent component analysis. J Neurosci Methods 134, 9–21, http://dx.doi.org/10.1016/j.jneumeth.2003.10.009.
Mutanen, T.P., Metsomaa, J., Liljander, S., Ilmoniemi R.J. In revision. Automatic and robust rejection of sensor noise in EEG and MEG: the SOUND algorithm.
Schlögl, A., Brunner, C. 2008. BioSig: a free and open source software library for BCI research. Computer 41, 44–50, http://dx.doi.org/10.1109/MC.2008.407.
