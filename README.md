# The Malaga-Streetview-Challenge Dataset
This is the public release of the Malaga Streetview Challenge dataset that is used in these papers to 
benchmark Visual Localization task under changing conditions:

```
Cinaroglu,  I.,  Bastanlar,  Y.:  
Image  based  localization  using  semantic  segmentation  forautonomous driving.  
In: 2019 27th Signal Processing and Communications ApplicationsConference (SIU), pp. 1–4. IEEE (2019)
```

```
Cinaroglu, I., Bastanlar, Y.: 
Training semantic descriptors for image-based localization. 
In:ECCV Workshop on Perception for Autonomous Driving(PAD). ECCV (23 August2020)
```

The dataset is based on the Málaga Stereo and Laser Urban Dataset (Downtown subpart) described in this paper:

```
Blanco-Claraco, J.L., Moreno-Duenas, F.A., J, G.J.: 
The malaga urban dataset: High-ratestereo and lidars in a realistic urban scenario. 
International Journal of Robotics Research33(2) (2014)
```

## A visual localization challenging dataset with wide-baseline based on a part of Malaga Urban Dataset

![pipeline](https://github.com/ibrahimcinaroglu/Malaga-Streetview-Challenge/blob/0ae489a642c10613e0a44a7dc84c827eb5aa0232/Streetview_Downtown_Samples.png?raw=true)

### Image Details
The RobotCar Seasons dataset uses images captured with the Grasshopper 2 Left, Right, and
Rear cameras mounted on the vehicle used to create the original RobotCar dataset. The 
images provided with the RobotCar Seasons dataset have been undistorted.
Below is a table mapping the images taken under different conditions to the capture dates
listed on the RobotCar [webpage](http://robotcar-dataset.robots.ox.ac.uk/). An extended 
version of this table is included in the extended version of the CVPR 2018 paper that can be
found on [arXiv](https://arxiv.org/abs/1707.09092).

Condition | Capture Date
------------|----------------
overcast-reference | 28 Nov 2014
dawn | 16 Dec 2014
dusk | 20 Feb 2015
night | 10 Dec 2014
night-rain | 17 Dec 2014
overcast-summer | 22 May 2015
overcast-winter | 13 Nov 2015
rain |  25 Nov 2014
snow | 3 Feb 2015
sun | 10 Mar 2015

### License
All files provided by Malaga-Streetview-Challenge dataset are licensed under a 
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/) 
license and are intended for non-commercial academic use.

Also note that, the images provided with the Malaga Downtown dataset originate from the Málaga Stereo and Laser Urban Dataset. 
They are licensed under MIT License and the new BSD license (MRPT). 


#### Using the Malaga-Streetview-Challenge Dataset
By using the Malaga-Streetview-Challenge Dataset, you agree to the license terms set out above.
If you are using the Malaga-Streetview-Challenge Dataset in a publication, please cite **both** of the
following two papers:
```
@inproceedings{ccinarouglu2019image,
  title={Image Based Localization Using Semantic Segmentation for Autonomous Driving},
  author={{\c{C}}inaro{\u{g}}lu, {\.I}brahim and Ba{\c{s}}tanlar, Yal{\i}n},
  booktitle={2019 27th Signal Processing and Communications Applications Conference (SIU)},
  pages={1--4},
  year={2019},
  organization={IEEE}
}

@article{cinaroglutraining,
	title={Training Semantic Descriptors for Image-Based Localization},
	author={Cinaroglu, Ibrahim and Bastanlar, Yalin},
	journal={ECCV Workshop on Perception for Autonomous Driving(PAD)},
	year={23 August 2020}
}
```
