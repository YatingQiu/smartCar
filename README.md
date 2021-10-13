# smartCar
The smart car is a highly computerized automobile featuring ubiquitous computing, intuitive human-computer interaction and an open application platform. Here, we propose an advanced Smart Car demonstration platform with a transparent windshield display and various motion sensors where drivers can manipulate a variety of car-appropriate applications in augmented reality. Similar to smartphones, drivers can customize their Smart Car through free downloads of car-appropriate applications according to their wants and needs. 
Additionally, three potential car-appropriate applications related to computer vision are investigated and implemented in our platform for increased driving safety. The first and second carappropriate applications aim to enhance the driving visual field by restoring the low-visibility scenes captured during inclement-weather or nighttime driving conditions to be high-visibility ones, respectively, and display them on a transparent windshield display. We also survey pedestrian tracking techniques that combine multiple driving recorders' information as a mobile surveillance network, including one proposed framework we have developed as the third car-appropriate application. By embedding these carappropriate applications, the Smart Car has the potential to increase safety of driving conditions both in daytime and nighttime, even in bad weather.

# Introduction
Ubiquitous sensors, devices, networks, and information are opening the door to a smart world in which smart devices have extended computational intelligence throughout the physical environment to provide reliable, relevant services to users. These devices are getting smarter, more multi-functional, and more customizable to allow users to access and store comprehensive information via many downloadable applications.

In general, the smart devices are characterized by three important properties:

Ubiquitous computing (ubicomp): assessing information or being assessed interactively and autonomously everywhere and anywhere via various sensors over different wireless protocols.

Human computer interaction (HCI): the essential interfaces of smart devices that offer an interaction between human and computer.

Applications platform: allowing users to download the third-party application (app) software for customizing their smart devices.

Thanks to these properties, smart devices can act as critical facilitator for the Internet of Things (IoT) through the use of recent information and communication technologies (ICT), such as mobile operating systems (e.g., Android, iOS, Windows Phone, etc.), multimedia interface, internet access (e.g., Bluetooth, NFC, Wi-Fi, 3G, 4G/LTE, etc.), mobile apps, digital cameras, global positioning system (GPS) sensors, motion sensors, and so on.

So what will the next generation devices be like? Let's take a look at the facts in terms of mobile phones and televisions. Mobile phones, which were truly the first pervasive transportable computer, have evolved into multi-service devices now called “Smartphones.” The prevalence of these computerized phones allows users to send photos, audio, written documents, and videos to contacts via their phones instead of just using their phones to make calls, as can be seen in Fig. 1(a). In recent years, these modern properties have also been enabling new television (TV) features, turning “dumb” TV into “Smart TV” that give users great potential to watch on-demand videos and access internet-based options via Smart TV's range of online applications (see Fig. 1(b)). Nowadays, the automobile can be regarded as an electronic system in addition to a mechanical one as it incorporates computers, informational storage, and software.

![image](https://user-images.githubusercontent.com/83450250/137088621-3913f9ef-6f56-424f-9a63-f945ae3f1677.png)

Figure 1. Lives before and after changes in technology for mobile phones, televisions, and cars. (a) Lifestyle brought by smartphones nowadays; (b) Lifestyle brought by smart TVs nowadays; (c) Lifestyle brought by Smart Cars in the future.

Looking beyond prevalence, we believe that in the near future such advanced properties will include more vehicle technologies, thereby turning “dumb” cars into “Smart Cars.” This may include transparent windshield displays (see Fig. 1(c)) to increase driver and passenger safety, convenience, and performance. Hence, the Smart Car should include the following properties:

Ubicomp for Smart Cars: The in-vehicle system should be networked, autonomously context-aware, and transparently accessible. Additionally, the system should be able to handle multiple datasets and interactions acquired quickly from various sensors.

HCI for Smart Cars: The windshield should be replaced entirely by a see-through display while embedding various sensors to convey information in a straightforward and easy manner.

Application platform for Smart Cars: The development platform should be opened up. Hence, several car-appropriate applications from third-party developers would allow users to customize vehicle capabilities and features for their wants and needs.

To illustrate our claim, we present a novel Smart Car demonstration platform (see Fig. 2) equipped with various sensors and a transparent windshield display to receive and display virtual information to driver. The Smart Car that can provide virtual managements of every detail in our lives and navigate everyday traffic in augmented reality for highway, urban streets, and unstructured scenarios, will become a reality in the next few decades. Additionally, we discuss three potential applications, including a visibility restoration application, a nighttime contrast enhancement application, and a driving environment understanding application, to enhance operational safety for Smart Cars when driving in urban street scenarios.

![image](https://github.com/smartCarLab/smartCar/blob/master/image/image1.png?raw=true)

Figure 2. Exterior and interior views of the Smart Car demonstration platform.

# Smart Car Platform
The system architecture of the Smart Car demonstration platform is divided into three major units (see Fig. 3):

The interaction unit, with a see-through windshield monitor to display content quickly instead of a traditional windshield, and with a variety of in-vehicle sensors to convey information to users or to the computing and communication unit.

The computing and communication unit, which provides access and execution of both external and internal services with internet access capability.

The application unit, which facilitates downloading of third-party apps.

![image](https://github.com/smartCarLab/smartCar/blob/master/image/image2.png?raw=true)

Figure 3. System architecture of the Smart Car demonstration platform.

A. Interaction Unit
In our Smart Car demonstration platform (see Fig. 4), there are two classes of input sensors to convey information about the environment outside the vehicle and the user's intended actions, and one class of output devices used to convey information about the feedback of the computing and communication unit.

Input sensors - vehicle surround sensors: There are six image sensors plus a GPS sensor around the Smart Car demonstration platform for capturing road scenes and locating the car's position. The configuration of these image sensors, which jointly offer the driver with a 360-degree view out of the vehicle, is given in the left side of Fig. 4.

Input sensors - user behavioral sensors: In our Smart Car demonstration platform, there are three kinds of motion sensors (including a gesture sensor, a voice sensor, and an eye-tracking sensor) mounted on the dashboard of the vehicle which receive user's commands and transmit them to the computing and communication unit, as shown in the right side of Fig. 4.

Output devices - transparent windshield display: The Smart Car demonstration platform has a transparent display built into its windshield. Hence, the windshield acts as a display that allows users to not only see through the screen but also show on-demand information with real-time display in augmented reality through this visual interface. Here, the on-demand information refers to the driver's requests regarding the content of Smart Car's applications which are made available to driver as needed.

![image](https://github.com/smartCarLab/smartCar/blob/master/image/image3.png?raw=true)

Figure 4. The Smart Car’s configuration.

B. Computing and Communication Unit
The computing and communication unit of the Smart Car should provide real-time access and execution of external/internal services and process multiple data sets acquired from varied sensors of the interaction unit. Hence, the growing complexity of in-vehicle systems requires: integration and cooperation of the software modules; multisensor data fusion; stable storage; capability of plug and play. Therefore, the in-vehicle computing system should include specific features, as listed in Table 1.
C. Application Unit
We gave the Smart Car an open platform where users are able to download applications from automobile companies, government/private utility providers, and insurance companies in order to customize the features, performance, and capabilities.

Table 1 Specific information of in-vehicle computing system.

![image](https://user-images.githubusercontent.com/83450250/137089015-212a8e96-7a37-4240-8005-97137bc033e0.png)

The applications in this platform can be manipulated through gestures, voice, and eyes. Additionally, the user interface of the transparent windshield display consists of a header container (upper portion of the screen), a content container (mid portion of the screen), and a footer container (lower portion of the screen), as shown in Fig. 5. The header container always displays information such as the status of the car, traffic information, weather conditions, etc. The content and footer containers show the complete and simplified content from the activated application, respectively. The application platform can be downloaded from.

Table 2 Icons of three potential applications for operational safety enhancement in the Smart Car demonstration platform. The first column represents the number of icons and the second column represents three potential applications.

![image](https://user-images.githubusercontent.com/83450250/137089123-0a4c46d6-c943-42c2-bc3d-4f3eee278b1f.png)

![image](https://github.com/smartCarLab/smartCar/blob/master/image/image4.png?raw=true)

Figure 5. Layout combination of the transparent windshield display

# Smart Car Applications
In this section, we implement and discuss three potential applications for Smart Cars related to computer vision which can be used to enhance operational safety. All these three applications were previously developed by the authors of this paper and were adapted to fit into this Smart Car demonstration platform. The icons used for these three applications are given in Table 2.

A. Visibility Restoration Application
Inclement weather, such as heavy haze, fog, sandstorms, and so on, can make driving quite difficult and dangerous. For instance, a driver may have trouble seeing the road clearly and need more time to make a decision to brake when driving in heavy haze conditions, as shown in Fig. 6. The ability to use a transparent windshield display that enhances visibility could alert a driver to potential dangers when his/her vision field is diminished in inclement weather conditions.

In general, visibility restoration of a single image can be performed by using the optical model. This model recognizes that the reflected light and distance are linearly correlated with the observed object and camera [8]. The intensity of a hazy image I from the observed object to camera can be represented by direct attenuation (including the intensity of haze-free image J and the intensity of transmission T) and airlight (including the global atmospheric light A):

![image](https://user-images.githubusercontent.com/83450250/137089853-7e22737e-0339-4361-9738-438aa071a646.png)

Let's assume a homogeneous medium and that the intensity of transmission T represents the amount of light reflected back to the camera from the particle surface in which transmission T can be determined as T=e−βd, where β is the medium attenuation coefficient and d is the distance between the camera and the particle surface. In particular, the aim of visibility restoration algorithms is to estimate the latent haze-free image J via transmission T from haze image I when there is no additional information available regarding depth and airlight. In practice, some driving situations may appear and disturb these visibility restoration algorithms. Here, we identified the following challenging situations in the field of visibility restoration for driving situations.

Local lights: When driving in hazy conditions, either the headlights of vehicles or the streetlights are usually turned on to improve the driver's vision field. This often causes misjudgement of airlight for some visibility restoration algorithms, resulting in artifact effects.

Colorcast problems: It is due to the different kinds of particles that absorb different portions of the color spectrum, and usually results in different distributions of color channels, thereby producing a restored image that still suffers from colorcast problems.

Gray road: The roadway is usually gray in images captured in the daytime. In foggy conditions, this may result in over-restoration of the road part of the image due to the similarity between the road color and the fog color.

Deep depth of field: Under hazy weather conditions, the haze is thicker across the vanishing point of the road than it is in front of vehicle (which is close to haze-free). When driving in situations with deep depths of field, the uneven haze density in the image might be misjudged by visibility restoration algorithms, thereby resulting in a restored image that still appears hazy.

Planar surface: Hazy images captured on roadways during driving conditions are generally assumed to be planar. As such, some visibility restoration algorithms are not able to effectively restore visibility in hazy images that were not taken along a planar surface.

Complex architecture: Complex architecture may exist along a road, such as pylons, streetlamps, etc. A restored image can easily suffer from halo effects along the edges of these structures.

Table 3 gives an overview of common problematic issues. In this article, we take a cue from reference when considering the frequent appearance of local lights and colorcast problems during driving conditions. In the literature, a haze removal approach was developed and consisted of a hybrid dark channel prior (HDCP) module, a color analysis (CA) module, and a visibility recovery (VR) module. In the HDCP module, a hybrid transmission map was produced to estimate the haze density while avoiding the misjudgement of local lights as atmospheric lights. The hybrid transmission map can be expressed as

![image](https://user-images.githubusercontent.com/83450250/137089931-ca8cac52-4350-4e74-ade2-5db91840692a.png)


where ω, α, and β are the constant factors and can be acquired according to; dΩ (I) and dμ(I) are the processes of dark channel prior on each color channel of haze image I using patches of sizes 3×3 and 45×45, respectively. Moreover, the colorcast problem was suppressed by the CA module, where the color adjustment γc for cth color channel was measured as

![image](https://user-images.githubusercontent.com/83450250/137090019-e96346a4-3f48-4078-84ef-51f3b38bed0e.png)

where mr(I) and mc(I) are the average processes on the R color channel and cth color channel in RGB color space, respectively.

Next, the VR module restored the haze image to haze-free one Jc by


where σc is the gain factor for cth color channel and can be produced by

![image](https://user-images.githubusercontent.com/83450250/137090172-05dbfc8f-f666-4ace-b73c-8165fbbb060d.png)

and l is the intensity level. Note that PMF(⋅) is the process of probability mass function and Ac is the atmospheric light for cth color channel obtained from dμ. In addition, the computational complexity of the haze removal approach is principally embodied in its three modules.

The complexity of HDCP module is O(kMN) to produce the hybrid transmission map for M row and N column via the patch size of containing k pixels. The complexities of both CA and VR modules are O(MN). After turning on the visibility restoration application (see Fig. 6), the vision field of the driver is improved, such that the driver can see the surrounding environment more accurately and engage in better decision-making.

Table 3 Challenges and solutions for visibility restoration algorithms in driving conditions. The first column lists the challenges and the second column lists the corresponding solutions.

![image](https://user-images.githubusercontent.com/83450250/137090273-50fdde76-d860-4b8e-9e58-cbc58eec0c4c.png)

![image](https://github.com/smartCarLab/smartCar/blob/master/image/image5.png?raw=true)

Figure 6. Manipulation of visibility restoration application in the Smart Car. Upper portion:
driving in conditions with poor visibility; mid portion: turning on the visibility restoration application;
lower portion: driver’s vision field has been improved after turning on the application.

B. Nighttime Contrast Enhancement Application
At night, the nighttime contrast enhancement application combines enhanced night vision with the transparent windshield display to allow drivers to both identify and highlight the location of threats (e.g., pothole or bump), as shown in Fig. 7.

![image](https://github.com/smartCarLab/smartCar/blob/master/image/image6.png?raw=true)

Figure 7. Driver performing the nighttime contrast enhancement application where the
driver’svision field is increased. Upper and lower portions represent the driver’s vision field
before and after using the application.

In general, the current image I captured by using imaging device consists of both the light reflectance R and the visible-light illumination L according to the literature. This can be expressed as

![image](https://user-images.githubusercontent.com/83450250/137090530-fec787c5-9ac9-43ff-a166-c9e551b485c1.png)

The light reflectance R would not be changed due to the illumination variance in the same scene. When the imaging device can receive sufficient illumination, the ideal illumination image Ii can be obtained by the ideal illumination Li. On the contrary, poor illumination Lp can produce a restored image with poor illumination Ip.

Table 4 Challenges and solutions for image contrast enhancement algorithms when driving at night. The first column lists the challenges and the second column lists the corresponding solutions.

![image](https://user-images.githubusercontent.com/83450250/137090599-d32cdf59-7b4b-4da3-baa2-f20216825ca2.png)

The main aim of various image contrast enhancement algorithms is to increase the illumination level via the processing function of contrast enhancement f(⋅), while preserving the image features. This can be expressed as follows:

![image](https://user-images.githubusercontent.com/83450250/137090652-879d9b75-32c1-4a92-b702-bee411560408.png)

Various algorithms have been developed to achieve the processing function of contrast enhancement. However, the use of these algorithms during nighttime driving conditions should specifically address the following issues:

Artifact tolerance: when driving at night, there are various light sources along the roadway to enhance a driver's vision field. The image contrast enhancement algorithms should avoid introducing certain artifacts (also called “blocking effects”) as the vehicle is moving.

Uniform contrast: the image contrast enhancement algorithms should be able to simultaneously and effectively enhance all portions of the current image during night-driving.

Brightness preservation: after the contrast of the current image is enhanced, the enhanced image should not lose the brightness of various light sources along the roadway.

Hence, several approaches have been proposed to overcome these issues, as listed in Table 4. In this article, we implement the nighttime contrast enhancement application by using algorithm for brightness preservation and artifact tolerance. In the literature, the adaptive gamma correction with weighting distribution (AGCWD) was proposed to enhance the image contrast for visual quality improvement. First, the transformation curve T of adaptive gamma correction was devised as follows:

![image](https://user-images.githubusercontent.com/83450250/137090712-86e71429-2cc7-47f8-b31c-64ee95abdba8.png)

where l and lmax are each intensity level and maximum level for an 8-bit pixel on V channel of HSV color model in a given image I, respectively. γ is the adaptive parameter for each level, which can be defined as

![image](https://user-images.githubusercontent.com/83450250/137090771-cb89002c-49ac-40a8-8295-b0a94c6a01bc.png)

where CDF(⋅) is the process of cumulative distribution function and can be expressed as follows:

![image](https://user-images.githubusercontent.com/83450250/137090849-3c79dd40-8966-4e4d-b9e4-41322a1ed4ed.png)

Next, the weighting distribution function W can be expressed as follows:

![image](https://user-images.githubusercontent.com/83450250/137090893-0992a0f7-41aa-4c55-a011-e0079fa8ec5a.png)

where α is an adjusted parameter, PDF(⋅) is the process of probability density function, and PDFmax and PDFmin are the maximum and minimum values of the statistical histogram in PDF(∀l), respectively. By using the transformation curve to the dimmed image in the application, the enhanced image potentially provides richer road information to the Smart Car's driver, as can be seen in Fig. 7. The overall efficacy of above processes on computational complexity is O(MN), where M and N are the number of rows and columns in a given image I, respectively. Therefore, a temporal-based entropy model was suggested in and employed to reduce the computational complexity for the visibility restoration application and nighttime contrast enhancement application. For tth frame, the entropy Et can be measured as follows:

![image](https://user-images.githubusercontent.com/83450250/137090947-3dbaf686-5a59-4fad-b23b-3b087b507e68.png)

Here, the first incoming frame is utilized to produce the hybrid transmission map and the transformation curve for these two applications at the beginning of their processes. This information will be recalculated only when the absolute difference between Et and Et−1 is higher than a predefined threshold δ, where δ can be set as 0.05 according to.

C. Driving Environmental Understanding Application
Thanks to increasing development of autonomous technologies, many video analytics applications are being applied to moving platforms such as Smart Cars. Human tracking is quite challenging since humans may vary greatly in appearance due to different viewing perspectives, non-rigid deformations, intra-class variability in shape, and other visual properties. The challenge increases when moving cameras (such as the car recorders) are employed, due to the effects of egomotion, blur, and the issues mentioned above. The introduction of a moving camera invalidates many effective moving object tracking techniques used in static camera, such as background subtraction and a constant ground plane assumption, thus making the task more difficult. Rather than using background modeling-based methods to extract captured human objects, human detectors are widely used to detect images of people in the video frame. Therefore, the challenge is to successfully detect human images captured by moving cameras, and then apply the tracking techniques to those detected, resulting in socalled tracking-by-detection schemes.

By applying a human detector to each frame of a video sequence, the tracking scheme becomes a task that associates the detected human objects with each other frame-by-frame. In general, human detection follows two basic steps: foreground segmentation and object classification.

After human object detection, a tracking framework is applied to the detected objects. Previous research of human tracking with moving cameras has involved Kalman filters, Particle filters, and kernel-based tracking, which are widely used in tracking and independently consider each tracked human within the temporal frames. Some studies adopt Multi-Hypothesis Tracking (MHT) and Joint Probabilistic Data Association Filters (JPDAFs) to optimize detected target associations by jointly considering all tracked targets' information over several time steps.

Alternatively, several approaches based on the structure-from-motion (SfM) framework have been developed. The SfM framework, when combined with visual simultaneous localization and mapping (V-SLAM), can be used to calibrate and localize the 3-D positions of the moving camera, and eventually detect, track, and reconstruct moving objects with respect to the static background. This results in a so-called dynamic scene reconstruction. The advantage of the SfM-based approaches is that they locate the objects in 3-D space, so as to better deal with occlusion issues during tracking. Table 5 summarizes several existing human tracking-by-detection schemes based on a moving camera, with or without 3-D inference.

A robust moving-platform-based human tracking system, which takes advantage of the tracking-by-detection scheme and successfully integrates V-SLAM, human detection, ground plane estimation, and kernel-based tracking techniques, is adopted in our Smart Car system. As shown in Fig. 8, this system starts with human detection and V-SLAM for camera calibration. Then, the ground planes are estimated based on the camera motions, so that the 3-D locations of the pedestrians (relative to the cameras) can be inferred. Subsequently, the absolute 3-D locations of tracked humans will become available since the GPS location information of the camera is also available. By taking 3-D information into account, the tracking problem can be reformulated as a constrained 3-D multiple-kernel (CMK) tracking problem, which can effectively resolve occlusions during tracking by globally optimizing the data association between consecutive frames.

![image](https://user-images.githubusercontent.com/83450250/137090998-988e15d9-25e8-4615-8ff5-b143833ca15c.png)

Figure 8.A moving-platform-based human tracking system.

In, the CMK tracking scheme tracks video objects in 2-D space (image), i.e., x∈R2×Nk in Eq. (16). To efficiently integrate the depth information into the CMK framework, we need to reformulate the problem. First we extend the Eq. (16) from 2-D to 3-D space

![image](https://user-images.githubusercontent.com/83450250/137091302-833b9a83-8453-46ae-977c-056f9a0f8029.png)

Table 5 Several existing human tracking-by-detection schemes based on a moving camera, with or without 3-D inference.

![image](https://user-images.githubusercontent.com/83450250/137091303-75ec71bc-5138-4340-8443-79b27f3712d2.png)

This equation is regarded as the local optimization for each individual target i with multiple (Ni) kernels, each of them is weighted by wik. Second, considering the depth information, we assign the visibility of each target as a weight vi to deal with the global optimization. In other words, the total cost function becomes:

![image](https://user-images.githubusercontent.com/83450250/137091301-ceb06137-80b0-4c5a-a232-1d422b32a247.png)

where M is the number of the targets in one video frame, and X=[(X11)T,…,(Xik)T]T is for the ith target and the kth kernel.

Necessarily, the constraint functions C(X)=0 must be considered to maintain the relative locations of the kernels. In, two-kernel and four-kernel layouts are proposed to describe a human. Unlike the constraints used in, which are mainly based on 2-D geometry, we set the constraints based on 3-D geometry. Hence, for each target i, the movement vector δx can now be iteratively solved by using the projected gradient method. The computational complexity is relatively high, due to the use of human detector on every frame of video, as well as the ground plane estimation. The CMK tracking in 3-D space based on projected gradient can be very fast. At this moment, using a high-end desktop CPU still requires couple seconds to complete one frame of video. This complexity can be relieved if the cloud computing with GPU speedup, real-time processing can be expected.

As examples, representative performances of human tracking for videos obtained from four separate car recorders are shown in the left column of Fig. 9. Moreover, a 3-D visualization of dynamic on-road scenes can also be reconstructed. Its purpose is not only to visualize the pedestrians' paths and movements in a 3-D environment, but also to avoid issues of privacy invasion by using avatar-like 3-D models. When effectively integrated with a 3-D map service, such as Google Earth, we can treat this new 3-D augmented reality visualization as a “dynamic 3-D GPS navigation” system as shown in the middle column of Fig. 9. When there is an event, such as road crossing or activity, we can see the dynamic scene in different aspects of views (see the right column of Fig. 9), which can be effectively displayed within the Smart Car to facilitate drivers' viewing experience.

![image](https://user-images.githubusercontent.com/83450250/137091300-71bc0df7-e2b8-4849-ae44-c75ab4582d23.png)

Figure 9. 3-D visualization of the scene recorded by four driving recorders. Each row belongs to one driving recorder; the leftmost shows the video frames, the middle shows the corresponding view of 3-D visualization, and the right shows the scene visualized from different aspects.

Moreover, due to the video analytics on each individual Smart Car, it is highly desirable to collectively combine analytics information, such as on-road pedestrian tracking, from multiple nearby vehicles to dynamically facilitate better monitoring of the on-road situation and cooperatively share the information. When tracking pedestrians in a Smart Car with a single moving camera, the camera's field of view (FOV) is limited to the front of the vehicle and dynamically changes when the vehicle moves. To achieve a more complete understanding of the car's surroundings, the tracking must be implemented across multiple moving cameras based on the results of the tracking in a single moving camera. The challenge is that appearance features extracted from the same pedestrian by different cameras may be inconsistent. There are two scenarios associated with tracking across multiple moving cameras: overlapping and non-overlapping FOV scenarios. In an overlapping FOV scenario, a pedestrian simultaneously appears in two or more different cameras' FOVs; therefore, re-identification issues can be facilitated by exploiting the cameras' relationship based on the overlapping views, so as to obtain consistent features from different cameras. In a non-overlapping FOV scenario, a pedestrian enters a camera's FOV then leaves, and later enters other cameras' FOVs, which do not share a common region with the previous FOV. The problem is more difficult due to dynamic environment, lighting changing and unexpected camera locations. Hence, the methods for tracking across multiple static cameras cannot be applied to the tracking across moving cameras. Moreover, both overlapping and non-overlapping cases may occur alternatively during tracking, thus making this task even more challenging.

To effectively deal with tracking across multiple driving recorders, we developed a framework to track on-road pedestrians recorded in the videos, where a cloud server is used to collect driving information of several nearby vehicles via a mobile surveillance network. First, pedestrian tracking in a single moving camera is applied to each video. Based on the single-camera-tracking results, we treat the problem of tracking across cameras as a multi-label classification task, which determines each target belonging to one or several cameras' FOVs by considering association likelihood of the target as calculated based on targets' motion cues and appearance features. When a target is out of a camera's FOVs, we predict the target's locations via an open map service such as Google Maps. Moreover, by using the Google Earth service, a 3-D visualization of a dynamic scene can be reconstructed to allow users to see a holistic view or different viewing perspectives of a 3-D scene reconstructed by multiple videos.

Figure 10 shows the system of the developed framework. First, pedestrian tracking, which produces the moving trajectory and associated features of the tracked person (tracklet) in 3-D space, in a single camera is applied to each video. The videos are then used to build Brightness Transfer Functions (BTFs) for compensating the color diversity of the cameras. After estimating the pedestrians' 3-D tracklets in each camera, the pedestrian tracking across multiple cameras is further applied, facilitated with the BTFs and map prior. Finally, the pedestrians' 3-D tracklets are summarized and visualized in the 3-D real-world environment based on an open map service like Google Earth.

![image](https://user-images.githubusercontent.com/83450250/137091427-4dfa4bb2-cca8-427b-bff5-ba63120259f5.png)

Figure 10. A system of human tracking across multiple moving car cameras.

As shown in Fig. 11, the pedestrians (in yellow and green bounding boxes) appearing in Camera 1's FOV are successfully tracked (in the same color boxes) later in Camera 3's FOV.

![image](https://user-images.githubusercontent.com/83450250/137091498-2e080b96-39a9-4662-b839-3478a853aec4.png)

Figure 11. Visual tracking results, where the top rows are the recorded frames, and bottom rows are the corresponding 3-D visualization. (a) Two human tracked frames from driving recorder-1. (b) Two human tracked frames from driving recorder-3.

# Conclusions
We proposed the demonstration platform for a Smart Car and further implemented three potential applications on this platform. To implement the Smart Car demonstration platform, we included three important properties. First, the Smart Car is networked and is able to process multiple datasets from various sensors based on the ubicomp property. Next, due to the use of the HCI property, the traditional windshield is entirely replaced on the Smart Car by a transparent windshield display on which the driver can see graphic information and interact with the car via embedded motion sensors. Finally, the application platform of the Smart Car is designed based on the platforms of smartphone and smart TV, is opened up for third party developers, and can be downloaded from. This Smart Car demonstration platform was tested on three proposed applications. Additionally, we have demonstrated the potential capability of a Smart Car to effectively implement and run these three applications during driving conditions. We believe that in the future there will be a great diversity of car-appropriate applications released on the application platform. At that point, the smart world's drivers can build their own Smart Car based on their wants and needs. Consequently, the Smart Car will provide not only a more interesting driving environment, but also a safer one.

