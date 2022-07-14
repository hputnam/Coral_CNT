Image J processing SOP

Image J Cube Processing: (see old PP for Images) 

Need plugins: Time Series Analyzer V3 (for cube data analysis)

The first numbers 640x512 are the pixel numbers (not micrometers)

Contrast: 
Shortcut: 
Control (or command) -> shift-> C  (“auto”) [equivalent to 99.99% on computer imager]
OR Path:  
Image -> Adjust -> Brightness/Contrast

Cmmd (or CNTRL) +/- => zoom

Can check exposure by scrolling over individual pixels
To add a scale bar, go to image > properties. Change unit to um and pixel width/height/depth to:
o	20x: 0.725 (0.6967)
o	100x: 0.149 (0.143)

Insert Scale Bar: 
Analyze -> Set Scale (see values above)
Analyze -> Tools -> Set Scale Bar
 

 

LookupTables:
Image-> LUT (lookuptable)
Colors image for compounding 


Cube Processing: 
Duplicate cube, save original: 
Image -> Duplicate -> Duplicate stack (check box)
 
Label each image by wavelength: 
Image -> Stacks -> label 
	Starting value : 950
	Inverval (wavelength increments): 4 (lamda)
You can process images (despeckle for figures but don’t use for data analysis - data manipulation!)
 
Can click play button in bottom left corner and will automatically scrub through like video. 

Create cube images: 
for 1 image from 1 wavelength image: Image -> Stack -> Duplicate (ie Range 1, Rename: Autofluorescence) 
For 1 image, compressed range of wavelengths: Image -> Stacks -> Z project (combines multiple images from stack into one) -> Avg Intensity (gets rid of noise)
Use two images to make composite: 
Image -> Color -> Merge Channels 

Can use up to 7 images (channels” and merge) – make sure all same bit size
	“image” -> “type” – choose bit size
Click “keep source image” to save originals  
 

(good to present composite & two colored originals); can also overlay WL 
Save as -> PNG for best quality images (tiff won’t save contrast settings; JPEG and PNG will)


Can save as AVI for movie or GIF for repeating movie 
 File -> save as -> AVI or GIF

To analyze spectral data: 
Need plugins: Time Series Analyzer V3 (for cube)
Time Series V3 Plugin 
Pick an ROI(circle shape) -> “t” or “Add”
Have one ROI highlighted -> “Get Average” 
Gives graph and column values -> select All and copy and paste into Excel (origin)
Add in wavelength in column to left, save the first column of data (delete AVG and err)
	(first and second columns are redundant)
Can save ROIs as zip files
 

Ie. Compare ROI with autofluorescence and ROI with CNTs

Can compare pixel intensities with histograms 
“analyze” -> “histogram” -> look at “mean”  (do for each image ie 950 and 1210)
(ie autofluorescence (950 image) here has 1413 and CNTs(1210 image) have 1331) 
 


Can also do a “Z projection” of entire cube to look at washout effect of autofluorescence 
(“image” -> “stacks” -> “zproject” – “max intensity”) Save as Jpeg (will save contrast setting)
(PNG will be black)
 


Save BB as Jpeg too to save contrast (PNG will be black otherwise)

3 way composites with WL, 950, 1210 (peak wavelengths) preferred over just 950 and 1210



