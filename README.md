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
International Journal of Robotics Research33(2). (2014) DOI: 10.1177/0278364913507326 
```
The original Málaga Stereo and Laser Urban Dataset (with subset Downtown) can be found 
[here](http://www.mrpt.org/MalagaUrbanDataset).


### Dataset Details

A visual localization (VL) challenging dataset 'Malaga-Streetview-Challenge', was prepared in order to 
test the performance of our VL methods carried out in the studies above. Differently from the known VL 
dataset, this dataset provides not only short/long term changes but also wide baseline as compared in the
following figure below. This newly generated evaluation set has been made publicly available and we believe
it will be useful for researchers studying in this field.

![pipeline](https://github.com/ibrahimcinaroglu/Malaga-Streetview-Challenge/blob/0ae489a642c10613e0a44a7dc84c827eb5aa0232/Streetview_Downtown_Samples.png?raw=true)

Malaga-Streetview-Challenge Dataset contains a reduced subset of publicly available Malaga Downtown Dataset
as the database images. These were collected on nearly 8 km. urban route visualized in the given figure below. To be able 
to include viewpoint variety and long term changes, we manually collected query images from Google Streetview within 
every 10-20 meter in the same 8 km. route in different times (1st row in the figure above). In total, Malaga Streetview
Challenge has 436 query images and 1561 database images (Rectified and decreased version of Malaga Downtown). Below is a 
table mapping the detailed statistics of the dataset.

![pipeline](https://github.com/ibrahimcinaroglu/Malaga-Streetview-Challenge/blob/45be5d641ebb2d9ee1bf75a79a0faef4d5e40032/Route_Of_Dataset.png?raw=true)

Baseline | Database images conditions (# images) | Query images conditions (# images) | Geotags
------------|----------------|----------------|----------------
Wide baseline | Reference traversal (Rectified and decreased version of Malaga Downtown) in 2014 - (Overcast/1561) | Google Streetview (436): all short-long term changes by different time period and years from 2014 to 2020 | Radian decimal latitude-longitude values in WGS84 geodetic datum

Corresponding geotags for images are also provided in radian decimal latitude-longitude values (Table above). Database image coordinates (1561) are obtained from the binary files that Málaga Stereo and Laser Urban Dataset provides us. Query image coordinates are manually collected from Google Maps.
Also it should be noted that, all these values are in WGS84 geographic coordinate system and It is known Google Maps also works with WGS84 geodetic datum. We have verifided that given GPS values are compatible with Google Maps coordinates.

A sample verification of same GPS information with its Google Stretview (left one) and Malaga Downtown (right one) image pair is given in the following figure below. 

![pipeline](https://github.com/ibrahimcinaroglu/Malaga-Streetview-Challenge/blob/bffbde30a7f6948d75c7ab59f89a0bde3dc1427e/Verification_Of_Geotag.png?raw=true)

## Provided Files
The following files are provides with this release of the Malaga-Streetview-Challenge dataset in various 
directories:
* `3D-models/`: Contains the 3D models created from the reference images.
* `extrinsics/`: Contains the extrinsic camera calibration between the three cameras used in
 the dataset.
* `images/`: Contains the images of the RobotCar Seasons dataset.
* `intrinsics/`: Contains the intrinsic calibrations of the three cameras used in the dataset.


 "all-sensors_GPS.txt " includes 1572 GPS records that corresponds to 1572 stereo images.
Each line contains an entry with the Longitude, Latitude and Height values in radians. 

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
### Privacy
We take privacy seriously. If you have any concerns regarding the images and other data
provided with this dataset, please [contact us](mailto:ibrahim.ceinaroglu@gmail.com).
