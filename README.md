# crs_scraper

### crs_scraper.py 
 - scrapes everything from the crs website then outputs a data in the form of list[dict[str, str | list[str]]]
 - TODO:
   - Still needs good user interface in the terminal 

<br />

### crs_data.py (for debugging purposes only, this is just temporary)
 - just contains the data itself for debugging

<br />

### data_sorter.py
 - input: the data from crs_scraper
 - outputs: all possible combinations of schedules with no time conflict
 - TODO:
   - Still needs a ranking system based on the chances generated by its available slots
   - Can be good as well if we can consider other constrains as well (e.g. Restrictions/Remarks) 

<br />

### crs_main.py
 - controls everything, including crs_data.py, data_sorter.py, crs_scraper.py
 - TODO:
   - Still need to link crs_scraper output here

<br />

## instructions for development
 1. Clone the repository
    ```
    git clone https://github.com/meezlung/crs_scraper.git
    ```

 2. Build docker
    ```
    docker build -t crs_proj
    ```

 3. Run docker
    ```
    docker run --name <insert-container-name-here> crs_proj
    ```

<br />

## Mga kulang pa:
 - Fix some property of schedules 
 - Ranking system
   - Based on available slots and demands  
   - RUPP Linking?  
 - App interface
 - I think we can organize while scraping na
