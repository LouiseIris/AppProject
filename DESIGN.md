# Design Document  
  
#### Sketch  
<img src=https://github.com/LouiseIris/AppProject/blob/master/advancedSketch1.jpg width="430"><img src=https://github.com/LouiseIris/AppProject/blob/master/advancedSketch2.jpg width="430">

#### Classes:  
Class LogInViewController:  
* Attributes:
  * emailTextField
  * passwordTextField
  * loginButton
  * registerButton
* Operarions:
  * log in with Firebase
  * alert with register
  * register with Firebase
  * to HomeViewController
  
Class HomeViewController:
* Attributes:
  * welcomeLabel
  * recipeImageView
  * recipeTitleButton
* Operations:
  * Suggestion function based on saved recipes
  * to DetailViewController
  
Class SearchViewController:
* Attributes:
  * ingredientTextField
  * searchButton
* Operations:
  * Autocomplete function with CocoaPods
  * to ResultsViewController
  
Class ResultsViewController:
* Attributes:
  * recipes
  * backButton
* Operations:
  * Retrieve function with API
  * to DetailViewController
  * to SearchVieController
  
Class DetailViewController:
* Attributes:
  * recipeTitleLabel
  * recipeImageView
  * ingredientLabels
  * descriptionLabel
  * backButton
  * saveButton
  * addButton
  * useButton
* Operations:
  * Save function: title and image url to Firebase
  * Add function: ingredient to Firebase
  * Points function: counts used ingredients
  * to ResultsViewController
  
Class SavedViewController:
* Attributes:
  * recipes
  * deleteSwipe
* Operations:
  * Delete function
  * to DetailViewController
  
Class GroceryListViewController:
* Attributes:
  * groceryItems
  * checkmark
  * deleteSwipe
  * addButton
* Operations:
  * alert for adding item
  * Add function: add item to Firebase
  * Delete function
  * Checkmark funtion
  
Class PointsViewController:
* Attributes:
  * points
  * savedLabel
  * leaderboardButton
* Operations:
  * 
  
Class LeaderboardViewController:
* Attributes:
  * users
  * points
  * backButton
* Operations:
  * HighestScore function to find users with most points in Firebase
  
#### API's and Frameworks:  
* Yummly API: https://api.yummly.com
* Firebase:
  * Authentication
  * Database for saved recipes
  * Database for grocery list
  * Database for points
* SerchTextField pod
  
