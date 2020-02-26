# Final Project of ML Techniques
### Problen Description

In this project, we are going to play with data from [Book-Crossing dataset](http://www2.informatik.uni-freiburg.de/~cziegler/BX/), which contains information of many user IDs, book descriptions and book ratings (integer value from 1 to 10). Instructor also provides the implicit book rating data (value 0) and hope you can make the best use of them if possible. Your goal is to predict the book rating, and you should notice that different tracks have different criteria. Besides the original Book-Crossing dataset, we additionally provide the external data crawled by TAs, which are the descriptions of some books (not all the books). Per course policy, you are **NOT allowed** to use any other data.

### Data Description

There are several files which contain all the information about the task:
* **user.csv**: The user ids and corresponding demographic data
  - User-ID: user IDs which have been anonymized
  - Location: demographic data (may contain NULL-value)
  - Age: demographic data (may contain NULL-value)
  
* **book ratings train/test.csv**: Containing the book rating information
  - User_ID: user IDs which have been anoymized
  - ISBN: International Standard Book Number which you can find some description through this (just like the Book ID)
  - Book-Rating: the book ratings range from 1 to 10 (Note that the test data would not have this value)
  
* **implicit ratings.csv**: Containing the book rating information
  - User_ID: user IDs which have been anoymized
  - ISBN: International Standard Book Number which you can find some description through this (just like the Book ID)
  - Book-Rating: all the book ratings are implicit, that is 0

* **books.csv**: Containing content information about books
  – ISBN: International Standard Book Number
  – Book-Title: content-based information
  – Book-Author: content-based information
  – Year-Of-Publication: content-based information – Publisher: content-based information
  – Image-URL-S: URLs linking to cover images (small size)
  – Image-URL-M: URLs linking to cover images (medium size) – Image-URL-L: URLs linking to cover images (large size)
  – Book-Description: TA-crawled descriptions of books
  
* **subimssion.csv**: Our book-rating predictions for testing samples
  - Book-Rating: the predicted book rating
  
### Evaluation
The submission website has two tracks of competition, each evaluated with a different goodnedd measure

* Track 1: [Mean Absolute Error(MAE)](https://en.wikipedia.org/wiki/Mean_absolute_error)
* Track 2: [Mean Absolute Percentage Error(MAPE)](https://en.wikipedia.org/wiki/Mean_absolute_percentage_error)

### Model
* Decision Tree
* Random Forest
* Adative Boosting

### Result
* Track1: Rank 5/21
* Track2: Rank 8/21
  
#### For other details, please refer to the file `project.pdf`
