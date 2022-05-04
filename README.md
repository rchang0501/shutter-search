# Shutter Search

Machine learning image recognition camera app built for Android that identifies the image using the Firebase ML Kit and provides search results of the identified image using the Google Search API, SerpAPI

<p align="center">
  <img src="/demo/icon.png" alt="shutter_search_icon" width="100" height="100"/>
</p>

### Tech Stack
**Languages**: Java </br>
**Libraries**: Jetpack Compose </br>
**Technologies**: Firebase, Android </br>

## App Usage 

### Step 1: launch app 
The UI of Shutter Search is a unique design of my own creation. The functionality is inspired by the popular app, Google Lens.

![Shutter Search Launch](/demo/1_launch.gif)

### Step 2: open camera 
Shutter Search requires permission to access the mobile phone's camera application to take a photo.

![Shutter Search Open Camera](/demo/2_camera.gif)

### Step 3: tap the shutter button to capture a picture   
The captured image is stored in a bitmap to display on the home screen and await identification. 

![Shutter Search Take a Picture](/demo/3_shutter.gif)

### Step 4: tap the search button to obtain search results    
First, using the Firebase ML Kit, the image is identified and labeled with a keyword of type `string`. Then, the keyword is queried using the Google Search API, SerpAPI. 

![Shutter Search Find Results](/demo/4_search.gif)

### Step 5: scroll through the search results!
Upon the SerpAPI query response, the JSON data is parsed and displayed within a horizontal recycler view to display all search results found with the keyword. 

![Shutter Search View Results](/demo/5_scroll.gif)
