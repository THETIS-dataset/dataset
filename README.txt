The dataset THETIS (Three dimEnsional TennIs Shots) was captured by a Kinect device. It consists of 8374 video sequences performed by 55 subjects, 31 beginners and 24 experts in playing tennis. Each sequence contains one type of action. There are 12 different classes of tennis actions : Backhand with two hands, Backhand, Backhand slice, Backhand volley, Forehand flat, Forehand open stands, Forehand slice, Forehand volley, Service flat, Service kick, Service slice, Smash.The scenes are indoor and there is a variety of background.

Each subject performs each activity two to four times and five types of video files are saved : 55x12x3= 1980 depth (.avi)  55x12x3= 1980, mask(silhouette) (.avi), 55x12x3= 1980 RGB (.avi), 1217 skeleton 2D (.avi), 1217 skeleton 3D (.avi). As far as the skeleton sequences are concerned, the calibration pose required for the extraction of the skeleton joints is not always successful, so skeleton sequences are fewer than other types of sequences.

There are five directories corresponding to the five types of recordings : Video_RGB, Video_Depth, Video_Mask, Video_Skelet2D, Video_Skelet3D.In each directory there are 12 subdirectories corresponding to the 12 different tennis actions.In each directory the file names have the format : {actor}_{action}_{sequence}.avi, where actor is the subject index, action is the action name and sequence is the index of the specific repeat.The correspondance between the names used for naming and the typical action names is : (backhand,Backhand), (backhand2h,Backhand with two hands), (bslice,Backhand slice), (foreflat,Forehand flat), (foreopen,Forehand open stands)(fslice,Forehand slice), (serflat,Flat service), (serkick,Kick service), (serslice,Slice service), (smash,Smash), (fvolley,Forehand volley), (bvolley,Backhand volley). The subject index ranges from p1 to p55.

As far as the VIDEO_Skelet3D and VIDEO_Skelet2D are concerned, we give a thorough description of the contents in each subdirectory.

Skelet2D :
1.backhand  {p7,p28,p33,p45}x0, {p1,p5,p6,p12,p13,p17,p18,p22,p29,p32,p40,p50}x 1,  {p2,p3,p23,p26,p46,p51,p53,p54}x 3 , 
2.backhand2hands  {p8}x0, {p11,p14,p23,p34,p55 }x 1, {p6,p20,p53}x 3,other subjects x 2
3.backhand_slice  {p8}x0, {p2,p7,p10,p12,p25,p27,p41,p43,p44,p47,p55}x 1, {p6,p20,p53}x 3, other subjects x 2
4.forehand_flat	  {p6,p19,p21,p32,p50,p55}x1, {p3,p4,p8,p11,p31,p49}x 3, other subjects x 2
5.forehand_openstands	{p7,p12,p15,p21,p22,p33,P35,p36,p58,p50,p52}x 1, {p3,p4,p9,p53}x 3, other subjects x 2
6.forehand_slice  {p6,p7,p28,p32,p33,p34,p35,p40,p44,p45,p47,p48,p49,p50}x 1,{p1}x 3, other subjects x 2
7.flat_service	  {p37,p50,p22,p55}x0, {p1,p3,p5,p7,p13,p33,p36,p41,p45,p51 }x 1, {p2,p40,p44,54} x 3, other subjects x 2
8.kick_service	  {p37}x0, {p3,p8,p21,p27,p28,p32,p45 }x 1, {p1,p7,p11,p17,p31,p44,p48,p49,p53} x 3, other subjects x 2
9.slice_service   {p37}x0, {p2,p7,p11,p12,p19,p22,p31,p36,p41,p45,p52,p55}x 1, {p21,p51} x 3, other subjects x 2
10.smash   {p11,p37,p45}x0, {p3,p22,p27,p32,p34,p43}x 1, {p5,p16,p25,p28,p42,p55} x 3, other subjects x 2
11.forehand_volley    {p32,p49,p50}x0, {p7,p12,p21,p26,p27,p33,p34,p36,p37,p43,p51,p52,p53 }x 1, {p30} x 3, 
12.backhand_volley    {p32,p37}x0, {p5,p21,p22,p27,p35,p37,p45}x 1, {p2,p13,p41,p48,p51} x 3, other subjects x 2


Skelet3D :
1.backhand  {p7,p28,p33,p45}x0, {p1,p5,p6,p12,p13,p17,p18,p22,p29,p32,p40,p50}x 1,  {p2,p3,p23,p26,p46,p51,p53,p54}x 3 , 
2.backhand2hands  {p8}x0, {p11,p14,p23,p34,p55 }x 1, {p6,p20,p53}x 3,other subjects x 2
3.backhand_slice  {p8}x0, {p2,p7,p10,p12,p25,p27,p41,p43,p44,p47,p55}x 1, {p6,p20,p53}x 3, other subjects x 2
4.forehand_flat	  {p6,p19,p21,p32,p50,p55}x1, {p3,p4,p8,p11,p31,p49}x 3, other subjects x 2
5.forehand_openstands	{p7,p12,p15,p21,p22,p33,P35,p36,p58,p50,p52}x 1, {p3,p4,p9,p53}x 3, other subjects x 2
6.forehand_slice  {p6,p7,p28,p32,p33,p34,p35,p40,p44,p45,p47,p48,p49,p50}x 1,{p1}x 3, other subjects x 2
7.flat_service	  {p37,p50,p22,p55}x0, {p1,p3,p5,p7,p13,p33,p36,p41,p45,p51 }x 1, {p2,p40,p44,54} x 3, other subjects x 2
8.kick_service	  {p37}x0, {p3,p8,p21,p27,p28,p32,p45 }x 1, {p1,p7,p11,p17,p31,p44,p48,p49,p53} x 3, other subjects x 2
9.slice_service   {p37}x0, {p2,p7,p11,p12,p19,p22,p31,p36,p41,p45,p52,p55}x 1, {p21,p51} x 3, other subjects x 2
10.smash   {p11,p37,p45}x0, {p3,p22,p27,p32,p34,p43}x 1, {p5,p16,p25,p28,p42,p55} x 3, other subjects x 2
11.forehand_volley    {p32,p49,p50}x0, {p7,p12,p21,p26,p27,p33,p34,p36,p37,p43,p51,p52,p53 }x 1, {p30} x 3, 
12.backhand_volley    {p32,p37}x0, {p5,p21,p22,p27,p35,p37,p45}x 1, {p2,p13,p41,p48,p51} x 3, other subjects x 2





