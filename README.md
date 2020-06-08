# Beamforming Chip Calibration using a Neural Network

**본 과제는 과학기술정보통신부에서 시행한 정보통신,방송연구개발사업의 결과입니다.**


This project aims to calibrate the beamforming chip system that has two inputs and two outputs using a fully connected neural network. The system has two inputs, input<sub>gain</sub> and input<sub>phase</sub>, both ranging from 0 to 31. It has two outputs, output<sub>gain</sub> and output<sub>phase</sub>. Outpug<sub>gain</sub>'s unit is dB and output<sub>phase</sub>'s unit is degree. 

The neural network has two inputs, output<sub>gain</sub> and output<sub>phase</sub>, and it outputs two values, which are the inputs of the system that will output, in the end, output<sub>gain</sub> and output<sub>phase</sub>. The network pre-distorts the inputs in order to get the correct outputs in the end.

<p align="center"> <img src="./images/predistortion.png"> </p>

calibration_tf.ipynb shows the system achieves 84% of accuracy when 400 data are used for training and 122 data are used for testing. The same approach can be applied in IQ mismatch calibration.
