# Complications: Features in Watch Face

   
Watch face! Sounds interesting. Let`s go ahead in understanding complications more in detail. Before that, you must be aware that this feature is supported only from Tizen 5.0 version onwards. In addition, there are number of developers from the Samsung gear team involved in creating watch faces. These developers can customize watch faces as per the requirement by choosing the required designs, colors, and features. There are number of developer-friendly features called Complications. Complications are tiny customizable widget that appears on the watch face to provide a personalized experience to the user. 
The following are the different types of watch faces:
   
This blog focuses on the following:
•	Importance of complication framework
•	Various types of complication data
•	Reason for introducing complications in watch face
•	Relation between watch face and complication provider service 
•	Customize design elements in watch face   
Why Complication in Watch Face?
Complication is an additional feature in watch face apart from telling time. This helps to enhance or simplify user’s life. Every watch face has one or more complications. However, several complications are available in timepiece, which includes simple date display to complex function such as tourbillon (mechanism found in mechanical watch). 

 
(Image source: https://www.amazon.com/Waterproof-Military-Electronic-Stopwatch-Luminous/dp/B01BA77L12 and Wikipedia.com) 
For example, battery indicator is a complication on a watch face.
What are Different Types of Complication Data Type?
The concept of Tizen complication framework involves in providing a common way of sharing data with the help of protocol APIs for complications and watch applications. The data types include short-text, long text, ranged value, time icon, and image.  
The following table lists various data types of the watch face application:
Data Types	 Notes

Short Text	Used to exactly show only one icon or short title:
   
Long Text	Long title is expected to be shown:
 
(Image source: Complications)

Ranged Value	Used to show the progress bar by specifying the range value:
 
(Image source:  https://images.app.goo.gl/xMQMz4ATBPXwYJX97)

Time	Used to show time:
 
Icon	Used when text is not required to be shown but instead icon is shown:
 
Image	Used to set the image path of the data type.

For more information, see Complication Data Types.
What is the Importance of Complications Framework?
Some third party native application developers have certain demands that they would want to display data other than time such as S-health data, weather, and so on. There is no other alternative way to share those data with the native application without complication framework.
As noticed, watch apps made by Gear Watch Designer (GWD) displays S-health data, but not a native application supporting only fewer complications. Hence, in large number of complications GWD does not play a major role.
Relation between Watch Face and Complication Provider Service 
Watch face requests to update complication data to the complication provider service. This complication provider service updates the complication data on the watch face.  For more information, see Watch Face Complications. 
For example, 
Chronograph: In the following image, you can see the lapsed time on the watch face. This lapsed time is nothing but complication type for the watch face.
 
(Image source: https://www.youtube.com/watch?v=jK6l6g3ChMM)
After obtaining information about watch face, let us go ahead in designing elements on watch face. 
How to Customize Design Elements in Watch Face?
Editable (Customize) is a feature in watch application that has come up with design elements, which includes color, font, and so on. This allows the editor to edit as per your preference.
Use Case
The following are the three different use cases:
	Customize “DIAL” on the watch face based on size of the number:
   
	Customize minutes and second “HAND” on the watch face based on color and size:

	   
	
	
	Customize complication feature “BATTERY” on the watch face based on font and text:
   


 
Complications - Do and Don’t 
Do	Don’t
Complication data must be large enough.
  
	Complication data available must not be so small for the user. Else, the user has to squint to read the complication data.
Style of the complications must be aligned with the watch face.	Complications must not feel out-of-place on the watch face.

Conclusion
In my opinion, complications on watch face would look great. These configurations of complications would stay on the watch face. Complication as a feature has both advantages and disadvantages. Thereby, provides additional benefit to the user.
