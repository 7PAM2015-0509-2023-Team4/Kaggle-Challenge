# Kaggle-Challenge

In 2912, data science skills are needed to solve a cosmic mystery involving the Spaceship Titanic, an interstellar passenger liner with 13,000 passengers. The ship collided with a spacetime anomaly, causing almost half of its passengers to be transported to an alternate dimension, similar to its predecessor 1000 years ago.

Task: To predict whether a passenger was transported to an alternate dimension during the Spaceship Titanic's collision with the spacetime anomaly.

Training data: Personal records for about two-thirds (~8700) of the passengers, are used as training data. Passenger details of the following features are given in the train.csv file.

<ul>
<li>PassengerId - A unique Id for each passenger. Each Id takes the form gggg_pp where gggg indicates a group the passenger is travelling with and pp is their number within the group. People in a group are often family members, but not always.</li>
<li>HomePlanet - The planet the passenger departed from, typically their planet of permanent residence.</li>
<li>CryoSleep - Indicates whether the passenger elected to be put into suspended animation for the duration of the voyage.</li> <li>Passengers in cryosleep are confined to their cabins.</li>
<li>Cabin - The cabin number where the passenger is staying. Takes the form deck/num/side, where side can be either P for Port or S for Starboard. </li>
<li>Destination - The planet the passenger will be debarking to.</li>
<li>Age - The age of the passenger.</li>
<li>VIP - Whether the passenger has paid for special VIP service during the voyage.</li>
RoomService, FoodCourt, ShoppingMall, Spa, VRDeck - Amount the passenger has billed at each of the Spaceship Titanic's many luxury amenities.</li>
Name - The first and last names of the passenger.
Transported - Whether the passenger was transported to another dimension. This is the target, the column you are trying to predict.
</ul>

Test data - Personal records for the remaining one-third (~4300) of the passengers are given in test.csv file.

About the new features: 
<ul>
<li> We identified 6 numerical features, 7 categorical features, and one target variable. </li>
<li> We extracted new features such as Group_Travel and Travel_Members from passengerID feature. </li>
<li> Group_Travel indicates whether each passenger travelled as a group or not and Travel_Members indicates the number of members each person travelled with. </li>
<li> Then we split the Cain feature into Deck/Cabin_No and Side. Finally, we extracted Name_length from the Name feature. </li>
</ul>

Feature transformations and scaling:<ul>
<li>The log transform was applied to remove the skewness of the below numerical features: ’RoomService’, ’FoodCourt’, ’ShoppingMall’, ’Spa’, ’VRDeck’</li>
</ul>
