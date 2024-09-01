# Portfolio_Data-Visualization

# My_Portfolio
Analytical and detail-oriented Data Analyst with a solid foundation in data analysis, statistical methods, and data visualization. Skilled in utilizing tools such as SQL, Python, Excel, Power BI. 

# [Project 1: Blinkit-Sales-Dashboar](https://github.com/DMNSHRMA005/Blinkit_Dashboard-files/blob/a3db04383da27fbdac6bacd4dc251ad9fb30930c/README.md)

### Dashboard
![Dashboard_upload](https://private-user-images.githubusercontent.com/96532941/363465431-ca964084-66a0-496d-9548-9b452b3d029e.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxNzQ1MTEsIm5iZiI6MTcyNTE3NDIxMSwicGF0aCI6Ii85NjUzMjk0MS8zNjM0NjU0MzEtY2E5NjQwODQtNjZhMC00OTZkLTk1NDgtOWI0NTJiM2QwMjllLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTAxVDA3MDMzMVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTMwOTk1M2NjYjllNGQ5ZTZlZDJlZmM1MDZjMTJhMWRmMjg1OTY0MGQ5ZTAxMDc0MmMyNGRjMzlkZmVhMDBkNDAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.A6g3KjwSvVfdV1BvLsc2KsrGvzsAhOnLUJFUg43B1_U)


## Problem Statement

This dashboard helps the Client understand their customers better. It helps the Client know if their customers are satisfied with their services. Through different ratings, Outlet Location, they get to know their improvement area, & thus they can improve their services by identifying these area. It also lets them know the average sales & departure time, thus since by using this dashboard they have identified this problem.

### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present except column named "Items weight".
- Step 5 : For calculating average delay time, null values were not taken into account as only less than 1% values are null in this column(i.e column named "Items weight") 
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Visual filters (Slicers) were added for four fields named "Outlet Location Type", "OUtlet Size" & "Item Type".
- Step 8 : Four card visuals were added to the canvas, one representing Total Sales Of Order & other representing Average Sales Blinkit was done & in other representing count of items and average Ratings we get on orders by consumers.
          Although, by default, while calculating average, blank values are ignored.
- Step 9 : A bar chart was also added to the report design area representing the number of Items conusmed by customers and with a bar chart we can check which products contains Low fat and Regular fat. 
- Step 10 : Ratings Visual was used to represent on which product we get different ratings mentioned below,

  (a) Baking Goods

  (b) Breads
  
  (c) Breakfast
  
  (d) Canned
  
  (e) Dairy
  
  (f) Frozen Foods

  (g) Fruits and Vegetables
  
  (h) Hard Drinks
  
  (i) Health and Hygiene
  
  (j) Household
  
  (k) Meat
  
  (l) Others
  
  (m) Seafood

  (n) Snack Foods

  (o) Soft Drinks

  (p) Starchy Foods
  
In our dataset, Some parameters were assigned value 0, representing those parameters are not applicable for some customers.

All these values have been ignored while calculating average rating for each of the parameters mentioned above.
- Step 10 : In the report view, under the insert tab, using shapes option from elements group a rounded rectangle was inserted & similarly using image option company's logo was added to the report design area. 
- Step 11 : New measure was created in which, Total Sales of Product is mentioned.

For creating new measure following DAX expression was written;
       
        Total Sales = SUM('BlinkIT Grocery Data'[Sales])

![Snap_Count](https://private-user-images.githubusercontent.com/96532941/363464951-133babab-8c2e-40ad-bc7b-7a85f8a0dd47.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxNzM3OTQsIm5iZiI6MTcyNTE3MzQ5NCwicGF0aCI6Ii85NjUzMjk0MS8zNjM0NjQ5NTEtMTMzYmFiYWItOGMyZS00MGFkLWJjN2ItN2E4NWY4YTBkZDQ3LmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTAxVDA2NTEzNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTdlYzIzZmU0ZDk3YzRkZGZjM2VjMWJkODBiMzNlYjBjM2I3Mzk4NGQ2OTNhMGIwZTYwN2JiMTIyNjM5ZTlhNjUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.IkiRZGLmxezSZLir0wsbhKCpSzotFOY4FJKuuHDRoyM)

A card visual was used to represent Total Sales.

- Step 12 : New measure was created to find No of Items.

Following DAX expression was written for the same,
        
        No of Items = COUNTROWS('BlinkIT Grocery Data')
        
A card visual was used to represent count of Items.

![Snap_Count](https://private-user-images.githubusercontent.com/96532941/363465087-b94f501f-9f18-4b15-bd91-78403203f740.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxNzQwMjksIm5iZiI6MTcyNTE3MzcyOSwicGF0aCI6Ii85NjUzMjk0MS8zNjM0NjUwODctYjk0ZjUwMWYtOWYxOC00YjE1LWJkOTEtNzg0MDMyMDNmNzQwLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTAxVDA2NTUyOVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQzYzNhNGM4YjBlMTgxOWYyMmIzMjM5ZjYwOTQ5NWMwZmRkODEwYTk3MGJkNDUxMjc1YjI4ZWM3ODRkZDk1MTEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Ghxptca9OfgEyyoxroRTbIvVPCqsjI-oc5dtpAoX7eU)

        
 - Step 13 : New measure was created to find Average Sales,
 
 Following DAX expression was written to find Average Sales,
 
         Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales]) 
 
 A card visual was used to represent this Average Sales.
  
 ![Snap_Percentage](https://private-user-images.githubusercontent.com/96532941/363465233-f7403335-9c3d-49e0-9fe3-4f5038c5e71d.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxNzQyNDUsIm5iZiI6MTcyNTE3Mzk0NSwicGF0aCI6Ii85NjUzMjk0MS8zNjM0NjUyMzMtZjc0MDMzMzUtOWMzZC00OWUwLTlmZTMtNGY1MDM4YzVlNzFkLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTAxVDA2NTkwNVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWJkNzM4N2EyNDk2ZTIxNmRmZjhmMjQ1Y2IwMTRlNmZhNzE0MGE2MjQ2ZTE0ZDE0MWEzZGFlYmNjNTFiNzVkZmYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0._iTUjvo9wmPu411oicxGI-_U09cYDMJdY8tjeFN55eQ)

 
 - Step 14 : New measure was created to calculate Average Ratings.
 
 Following DAX expression was written to find Average Ratings,
 
         Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating]) 
    
 A card visual was used to represent this Average Ratings.
 
 
 ![Snap_3](https://private-user-images.githubusercontent.com/96532941/363465234-7c7e3668-884a-435e-9147-e763c0fe55a8.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxNzQyNDUsIm5iZiI6MTcyNTE3Mzk0NSwicGF0aCI6Ii85NjUzMjk0MS8zNjM0NjUyMzQtN2M3ZTM2NjgtODg0YS00MzVlLTkxNDctZTc2M2MwZmU1NWE4LmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTAxVDA2NTkwNVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQzZmQyMGNmNjM3NTBjMzkyMWIwM2M3NGZiMWY5OGQ5NzRjZDhjZTA5Y2IxOTQ3ZDRjM2ZkOTQ3Y2E4NGJiZGYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.ElgT8cpDDnJlIwkeRvXBG36xEW3-fbaMo11IPOQhfM8)
 
# Report Snapshot (Power BI DESKTOP)

 
![Dashboard_upload](https://private-user-images.githubusercontent.com/96532941/363465431-ca964084-66a0-496d-9548-9b452b3d029e.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxNzQ1MTEsIm5iZiI6MTcyNTE3NDIxMSwicGF0aCI6Ii85NjUzMjk0MS8zNjM0NjU0MzEtY2E5NjQwODQtNjZhMC00OTZkLTk1NDgtOWI0NTJiM2QwMjllLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTAxVDA3MDMzMVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTMwOTk1M2NjYjllNGQ5ZTZlZDJlZmM1MDZjMTJhMWRmMjg1OTY0MGQ5ZTAxMDc0MmMyNGRjMzlkZmVhMDBkNDAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.A6g3KjwSvVfdV1BvLsc2KsrGvzsAhOnLUJFUg43B1_U)


![Dashboard_upload](https://private-user-images.githubusercontent.com/96532941/363465609-38d9b159-add5-45bb-8698-b7dcbe9b9fcc.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxNzQ3MjEsIm5iZiI6MTcyNTE3NDQyMSwicGF0aCI6Ii85NjUzMjk0MS8zNjM0NjU2MDktMzhkOWIxNTktYWRkNS00NWJiLTg2OTgtYjdkY2JlOWI5ZmNjLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTAxVDA3MDcwMVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTE5YWZiOGVhYjcwMzA5ZjlhZjE0YjkyOGIxMGM0ZTI1ZDk5ZGNmMGEwMjhjYmQ1ZGQyOGRkMDk4ZGRkYzNhYjYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.q22Gd1YlawpbsPcYjz7v8RioYFTW0anxCNI7l9MxrdU)

# [Project 2: NetFlix Movies and TV Shows Exploratory Data Analysis(EDA) ](https://github.com/DMNSHRMA005/Portfolio_Data-Visualization/blob/2590e337edcdea4e31924ca2974f03fc0918ba0d/netflix-exploratory-data-analysis.ipynb)
This Project is done on Google Colab and is mainly based on Python. In this Project, I’ve found some correlations between different fields of the given dataset and I've also done some visualizations highlighting the given data.

* This Project is based on Movie Industry.
* The project is mainly based on pandas(for data cleaning), numpy(for statistics), seaborn and matplotlib(for data visualization).
* Some of the visualizations from the project:

![Count Plot]([https://private-user-images.githubusercontent.com/96532941/363468574-1715eb32-1710-4373-b794-4c8e369288c1.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxNzU5MjIsIm5iZiI6MTcyNTE3NTYyMiwicGF0aCI6Ii85NjUzMjk0MS8zNjM0Njg1NzQtMTcxNWViMzItMTcxMC00MzczLWI3OTQtNGM4ZTM2OTI4OGMxLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTAxVDA3MjcwMlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTAzNWI0OTBiOTcyMjZlMjljMzQ3MjhmZWRjYTA5ZDVmNjUyZWU3MjliMDQ3MzhmOGQyZjVjMDIwMTBmMDQyYTcmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.sKAKQCHxdxcVza-lmobTVf2q7ZT17Emdvo22yE1JdyI])
![Bar Graph]([https://private-user-images.githubusercontent.com/96532941/363468563-9e31ef85-20b0-47c1-8499-5ad44f151744.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxNzU5MjIsIm5iZiI6MTcyNTE3NTYyMiwicGF0aCI6Ii85NjUzMjk0MS8zNjM0Njg1NjMtOWUzMWVmODUtMjBiMC00N2MxLTg0OTktNWFkNDRmMTUxNzQ0LmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTAxVDA3MjcwMlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTljNzJmYjQ0OTBjYWFkZWVkMGJjZjliYmFmODdlNzA0ZDAwNTY2NzhjMWIzZmNkYTAzZGQ3ZTVjMTkwZDg5MDgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.bIys1vCfwzEQj8tjDArlT54I0e21pWarj9uoUlcxZVE])
![scatter]([https://private-user-images.githubusercontent.com/96532941/363468570-00d5af52-9da4-4a30-b70a-3788e0ad6ce1.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxNzU5MjIsIm5iZiI6MTcyNTE3NTYyMiwicGF0aCI6Ii85NjUzMjk0MS8zNjM0Njg1NzAtMDBkNWFmNTItOWRhNC00YTMwLWI3MGEtMzc4OGUwYWQ2Y2UxLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTAxVDA3MjcwMlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWNhNjk1YWRlYTUyY2VmMTk0MTMwZjdhNmQyODU5M2RkNmI1Y2QyZTJkZjNjM2RhMDNlY2MwZjM2MzI4YjBjM2EmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.-zrO40RqjArWnmfHBBUES79jRs3UrOy4zrXJOekEW10])
