# Boot-Camp-Project-2
The sources of data: 
	Web Scrape from Rotten Tomatoes ( https://www.rottentomatoes.com/ )
	Netflix Movies & TV Shows (https://www.kaggle.com/datasets/shivamb/netflix-shows)

Transformation of Data:
At first, we attempted to load the data from Rotten Tomatoes using Jupyter Notebook, however we ran into an issue of only being able to extract 32 movies at a time. We were able to code the computer to clicking the “Load More” button on the website to extract the entire list. Totaling 601 pages.
 
<img width="473" alt="image" src="https://user-images.githubusercontent.com/94650193/161600537-72f43251-410d-4e59-9a13-22adb28ce541.png">


We then tested the headers for the data frames. Assuring we retrieved the data we were looking for. Movie Title, Score and Release date. We were then able to print movies_df with over 9000 lines of data.
 
<img width="330" alt="image" src="https://user-images.githubusercontent.com/94650193/161600567-d2261ed4-a6ac-44ac-881d-013c599b12eb.png">

<img width="286" alt="image" src="https://user-images.githubusercontent.com/94650193/161600599-3a893761-0790-42ed-a2ac-7391133937c5.png">


The next steps involved importing data from a CSV file we downloaded from Kaggle, Netflix Titles. In the same lines we changed the title on the CSV file. We also merged both tables into one data frame.
 
<img width="498" alt="image" src="https://user-images.githubusercontent.com/94650193/161600626-6098df68-fcf1-4865-bc08-91725b87e9f1.png">
	








Next, columns were created using PostgreSQL. We were able to see how may data points were in the columns. We were also able to print the data frame.

<img width="464" alt="image" src="https://user-images.githubusercontent.com/94650193/161600660-433caaee-0069-4f45-8132-5c3aa279fb6b.png">



Next we combined columns, release_date from Rotten Tomatoes and Month_Day for the CSV file. We also concatenated the year from release_year. After that, we dropped columns Month_Day and release_year.
 
<img width="498" alt="image" src="https://user-images.githubusercontent.com/94650193/161600721-102a8ccd-4470-4890-89bb-1335ce388e47.png">

<img width="498" alt="image" src="https://user-images.githubusercontent.com/94650193/161600780-e19d1ddd-1b2b-49f1-8bf6-f4035be17e9e.png">


Next, we used str.replace for the duration column, to show in minutes. 
 
<img width="498" alt="image" src="https://user-images.githubusercontent.com/94650193/161600799-ca45eeb2-1235-4f3a-937c-f0da8153d729.png">
	


Next, we changed the data type of Score and duration from str to int. Then we displayed the data frame info.
 
<img width="310" alt="image" src="https://user-images.githubusercontent.com/94650193/161600821-2b70e6d0-b895-47d1-a867-c31d88482685.png">


Next, we displayed the data frame for the final verification of all data we wanted to display.

<img width="498" alt="image" src="https://user-images.githubusercontent.com/94650193/161600859-93f06841-2fff-458d-91c3-3cf4cc3a0eb6.png">


  
The final steps were loading the data back into PostgreSQL.

<img width="498" alt="image" src="https://user-images.githubusercontent.com/94650193/161600885-45feccce-e4f2-4b43-8824-11f53109ecfd.png">
