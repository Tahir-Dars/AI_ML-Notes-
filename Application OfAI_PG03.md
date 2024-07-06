A key application of AI is computer vision, where one can train a machine to identify content in images. This process is akin 
to how the human eye processes images.
## Diagnosing Diabetic Retinopathy
Retinopathy is typically diagnosed by an optometrist or ophthalmologist, who examines the patient's retina image (captured through
 methods like fundoscopy or fundus photography) to determine its health status. The practitioner identifies specific features such
 as clots or hemorrhages.When training an application to diagnose retinopathy, a programmer inputs thousands of healthy and diseased
 retina images. Each image is labeled as healthy or diseased, along with disease severity (from mild to severe). The application uses
 filters to extract image features. Through training, the application learns optimal filters that enhance features distinguishing healthy
 and diseased retinas. Once trained, the application can diagnose new retinal images using these learned filters.

![ch04](https://github.com/Tahir-Dars/AI_ML-Notes-/assets/150343129/44857c95-7d6e-4731-8dbb-9ef2c466ab0d)
___________________
___________________
Images are stored in a computer as pixel values, where a grid of numbers represents a grayscale image. Each cell in the grid is a pixel
with a value between 0 and 255. For example, a 6x6 grid of pixel values represents an image.

![ch04_1](https://github.com/Tahir-Dars/AI_ML-Notes-/assets/150343129/128ebcc9-9ec1-4ec3-989a-ad937c0f4b6b)

Applying this filter to the 6x6 image results in a smaller, easier-to-work-with image that still retains important features. This process enhances certain features, making it easier to recognize image content.






