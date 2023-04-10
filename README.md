# hackmates
Graphical Password Authentication
GRAPHICAL PASSWORD AUTHENTICATION

The user is required to select some images (let’s say different chocolates) in a specific pattern (for example dairy milk is followed by 5 stars which is in turn followed by KitKat and so on). Next time the user tries to log in, the images would have been shuffled, but the user will be required to follow the same pattern which was used initially. Every time the user will have to use the same sequence while the images are placed in different ways. This type of authentication is difficult to break since neither brute force nor dictionary attacks could breach it. It is used in various banking sites to add an extra layer of security.
The user is provided with multiple pictures and is supposed to select only particular images in a particular order in order to login. This way along with the traditional user-id and password, an extra layer of security is added which prevents it from brute force or dictionary attacks. 

Explanation:![image](https://user-images.githubusercontent.com/115423168/230960009-461b974a-60bc-4b43-abb7-4f137a257d31.png)

  

Here we’ve added different checkboxes with their particular ID’s and also respective three submit buttons. Each checkbox is assigned to a particular image and is held to that particular image only.
The user is supposed to checkbox the respective checkbox for the image and check any three images out of five and once they select an image, they can submit that particular image with the respective submit button, i.e., after the user selects the first image, they can click the first submit button and that will be held first in the image out of 3 images and respectively for other images. 
![image](https://user-images.githubusercontent.com/115423168/230960059-446e7864-4a8e-4ab6-aa98-5557d3986748.png)

 

Here we have created a function which shuffles the images (with their respective checkboxes) when the user hits the refresh button. This is done so that every time the user visits the website or refreshes the page, they are given a new order of shuffled images from which they have to select the images in the defined order. This makes sure that user does not remember the images in order they’re displayed but in the order they are defined to be selected in order irrespective of where they are placed in the page.
![image](https://user-images.githubusercontent.com/115423168/230960086-0d7d60e5-1e04-455f-b307-251294813844.png)


 

This part of code makes sure that user cannot select more than 3 images out of 5. This prevents accidental selections as the user can only check mark any 3 checkboxes of the respective images and the rest checkboxes won’t be selected (images won’t be selected).
 

These are the functions which will be triggered after clicking the submit buttons. The logic behind the functions is that when the particular checkboxes which are supposed to be selected are selected, a counter variable will be incremented by one value otherwise the counter variable remains with the default value as zero. After selecting the first image the user clicks the first submit button and if the image is same which was supposed to be selected (checking that with checkbox ID’s) the counter variable is incremented with one value. Similarly for second and third image and once the user has selected all the images, they are supposed to click the final submit button and if the counter variable’s value is three (counter variable’s value incremented thrice for three images if correct otherwise remains the default as zero) then it will be displayed through a alert box that the input of images is correct otherwise incorrect.
