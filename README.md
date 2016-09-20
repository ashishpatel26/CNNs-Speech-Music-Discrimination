# CNNs:Speech-Music-Discrimination

##Synopsis
This project describes a new approach to the very traditional problem of Speech-Music Discrimination. According to our knowledge, the proposed method, provides state-of-the-art results on the task. We employ a Deep Convolutional Neural Network (_CNN_) and we offer a compact framework to perform segmentation and binary (Speech/Music) classification. Our method is unchained from traditional audio features, which offer inferior results on the task as shown in (--reference to the paper--). Instead it exploits the highly invariant features produced by CNNs and opperates on pseudocolored RGB frequency-images, which represent wav segments. 

**We offer a mechanism for:**
 * Audio segmentation using the [PyAudio](https://github.com/tyiannak/pyAudioAnalysis.git) analysis lybrary
 * CNN training using the [CAFFE Deep-Learning Framework](https://github.com/BVLC/caffe)
 * Audio classification using: 
  * CNNs
  * CNNs + median_filtering 
  * CNNs + median_filtering + HMMs

##Installation
- Dependencies
 1. [PyAudio](https://github.com/tyiannak/pyAudioAnalysis.git) 
 2. [CAFFE Deep-Learning Framework](http://caffe.berkeleyvision.org/installation.html)
 
_* Installation instructions offered in detail on the above links_

##Code Description

* **Data Preparation**

   Split you data into train and test as shown in Fig1:
 
   <img src="https://github.com/MikeMpapa/CNNs-Speech-Music-Discrimination/blob/master/train-test.PNG" width="500" height="300">
   <figcaption>Fig1. - Data Structure</figcaption>

    * Train/Test and Classes represent directories whereas Samples represent files
     
    * Data should be pseudo-colored RGB spectrogram images of size 227x227 as shown in Fig2
    <img src="https://github.com/MikeMpapa/CNNs-Speech-Music-Discrimination/blob/master/sampleIMg.png" width="227" height="227">
    <figcaption>Fig2. - Sample Spectrogram</figcaption>
  
* **CNN Training** 
  1. Provide Network Architecture file ([_SpeechMusic\_RGB.prototxt_](https://github.com/MikeMpapa/CNNs-Speech-Music-Discrimination/blob/master/SpeechMusic_RGB.prototxt) ).
     You can use any other CNN architecture of your choice. This one is the proposed architecture as described in the paper. 
   

##Code Example
--how to run and outputs

##Contributors

##References


##Cite
