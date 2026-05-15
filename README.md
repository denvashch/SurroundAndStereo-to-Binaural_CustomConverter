**CODE**

"Extract_brir" and "RIR" jupyter notebooks contain Python algorithms for deconvolution of BRIR and RIR measurements. Both programs process and save the extracted impulse responses to paths pre-determined by the user. The only expected audio inputs are WAV files featuring logarithmic sine-sweep measurements associated with BRIRs or RIRs.

"Code" contains Python code for stereo/surround to binaural conversion algorithm. It can accept either 6 audio inputs corresponding to 6 surround 5.1 format channels or 1 stereo 2-channel input and offers two rendering modes: 1) based on BRIR (binaural room impulse response); 2) based on combimation of HRTF (head-related transfer function) and RIR (omnidirectional room impulse response). Individual BRIRs, RIRs, or HRTFs (HRIRs) associated with each channel, as well as the headphone compensation filter, can be determined and loaded by user in a dedicated pre-processing section. RIRs and BRIRs were measured at New York University. 
    Note 1) Users also can use an IRslicer to appropriately isolate impulse responses from deconvolved sine-sweep measurements. It features tail length and fade out parameters, allowing for  customized isolation and modification of the acoustic properties of late reverberation.
    Note 2) In the standard 5.1 surround configuration, all inputs have the same duration. In this converter, surround inputs can be of any sample length, allowing for experimentative and/or more efficient approaches to audio processing.
    
**FILES AND MEASUREMENTS**

"Source" folder contains the 5.1 surround and stereo audio files which were sources for renders used in the perceptual study. It also features seperate folders for unprocessed original BRIR and RIR measurements made at the New York University James Dolan Music Recording Studio.

"RIR" and "BRIR" folders contain impulse responses extracted from the measurements using the original deconvolution algorithms implemented in "Extract_brir" and "RIR" jupyter notebooks. 

"Renders" folder contains surround-binaural/stereo-binaural renders (BRIR and HRTF+RIR) made with the source files for the perceptual study. 




