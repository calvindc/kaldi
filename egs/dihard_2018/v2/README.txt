 This recipe is the speaker diarization recipe for The First DIHARD Speech
 Diarization Challenge (DIHARD 2018). There are two tracks in the DIHARD 2018 
 competition , one uses oracle SAD (track1) and the other required that SAD 
 was performed from scratch (track2). This script is for track1.

 The recipe is closely based on the following paper:
 http://www.danielpovey.com/files/2018_interspeech_dihard.pdf but doesn't
 contain the VB refinement. The whole system mainly contains training and
 extract x-vectors, PLDA scoring and agglomerative hierarchical clustering. 
 The VoxCeleb datasets are used for training x-vectors and PLDA. The
 development set of the DIHARD 2018 competition is used as validation set to
 tune parameters. The system is tested on the DIHARD 2018 evaluation set. 

 We also use the following datasets for augmentation.

     MUSAN               http://www.openslr.org/17
     RIR_NOISES          http://www.openslr.org/28
