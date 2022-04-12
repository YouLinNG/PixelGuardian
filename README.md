# Usage

1. Follow the link https://cloud.google.com/vision/docs/detecting-safe-search#vision_safe_search_detection
2. Create a Google cloud project and enable the Vision API
3. In the Demo.ipynb replace the json key with your own Google Project json file

```python
def detect_image(path):
    # Google SafeSearch Detection API detects explicit content such as adult content or violent content within an image. 
    # This feature uses five categories (adult, spoof, medical, violence, and racy) and returns the likelihood that each is present in a given image
    os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = "YOUR OWN JSON FILE"
    import io as ios
    client = vision.ImageAnnotatorClient()
```

4. The parameter 'path' in detect_image function and pixel_image function is the path to your local image 
