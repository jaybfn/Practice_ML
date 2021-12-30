**** Classifying Artist's lyrics using Supervised Machine Learning ****

Steps:

1.In this project I am extracting lyrics of 6 artists ['Eminem','Jay-Z','Justin-Timberlake','50-Cent','Bob-Marley','Michael-Jackson'] from lyrics.com (# of artist can be any length)
2.For scraping lyrics please run 'cli_get_lyrics' on your command line interface.

	eg: type the below line on your command line interaface with path where your python file is located.
		
	> python cli_get_lyrics.py 6 --list Eminem Jay-Z Justin-Timeberlake 50-Cent Bob-Marley Michael Jackson
		> if you just run the file without giving any input arguments, then the code would function with its defaul values stored:
			> default val: number of artist is "1" and name of hte artist is "Akon".

	> python is the language I am using to scrap and classify lyrics 

	> cli_get_lyrics.py is the file which contains webscrapping protocols to scrap lyrics from 'lyrics.com'

	> the file 'cli_get_lyrics.py' required two input arguments to function.
		> number of artists to be scrapped( in my case I have 6)
		> name of the artists as mentioned on the lyrics.com (--list Eminem Jay-Z Justin-Timeberlake 50-Cent Bob-Marley Michael Jackson)

	> Once scrapped, the program will store all the lyrics as .txt file in individual folder with artist names
		> eg: I scrapped 100 songs from Akon, so there will be a folder with name Akon and 100 lyrics stored in it.

	> the program take cares of all the duplicate file name and repeated lyrics.

	> to abort the program in between press ctrl + c to interrupt.

3. Once all the lyrics are scrapped! Next, open Lyrics_Classification_RFC_25Dec2021
	
	> this code required two input arguments:
		> folders = ['Eminem','Jay-Z','Justin-Timberlake','50-Cent','Bob-Marley','Michael-Jackson']
		> base_url = r"C:/Users/Asus/OneDrive/Desktop/Spiced_Academy/naive-zatar-student-codes/week4/"
			> folders is required as an input list (all the folder names of artist)
			> base_url is the path where the lyrics folder are saved.

4. It is important to note that this model i optimized for the above mentioned artists, so please feel free to optimize the hyperparameter of the model while using diferent artists.


Libraries used:

> cli_get_lyrics.py
	1. Requests
	2. re
	3. os
	4. pandas
	5. argparser
	6. sys
	7. BeautifulSoup

> Lyrics_Classification_RFC_25Dec2021

	1. pandas
	2. Numpy
	3. sklearn
	4. nltk
	5. string
	6. re, os
	
