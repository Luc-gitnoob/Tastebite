Here’s how you can update the README to include these details:

---

[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/JTy-CUJF)

# Project Assignment: Zomato Restaurant Listing & Searching

## Key Use Cases

### Data Loading
Create an independent script to load the Zomato restaurant data available [here](https://www.kaggle.com/datasets/shrutimehta/zomato-restaurants-data) into a database.
An independent script is used to load the Zomato restaurant data into a MySQL database. The script, located in the `Config.java` file of the backend, scrapes JSON and CSV files and loads the data accordingly. The file path is:
```
server/src/main/java/com/zomato/zomato_app/config/Config.java
```

![script](https://github.com/user-attachments/assets/fb4e336f-443b-47d2-a3ee-b469f0af268b)


### Web API Service

Develop a web API service with the following endpoints to serve the content loaded in the previous step:
- **Get Restaurant by ID**: Retrieve details of a specific restaurant by its ID.
  - **Endpoint**: `api/restaurants/{id}`
  - **Description**: Fetches details of a restaurant using its unique ID.
  - ![image](https://github.com/user-attachments/assets/d736833f-9800-426a-a68e-7b8511c5e6f8)
  
- **Get List of Restaurants**: Fetch a list of restaurants with pagination support.
  - **Endpoint**: `api/restaurants/?page=0&size=5`
  - **Description**: Retrieves a paginated list of restaurants. You can adjust the `page` and `size` parameters to navigate through the list.
  - ![image](https://github.com/user-attachments/assets/95030271-c815-42ee-8fe7-88a44c5ed967)


### User Interface
Develop a web application with the following pages, which must connect to the web API service:


#### Restaurant List Page
Display a list of restaurants. Clicking on a restaurant should navigate the user to the restaurant's detail page.
![Restaurant List Page](https://github.com/user-attachments/assets/d7c094e0-3e2a-4787-9fa3-6ada8f2980de)


#### Restaurant Detail Page
Show details of a specific restaurant.
![Restaurant Detail Page](https://github.com/user-attachments/assets/a1275d5f-ec3d-4220-b1dd-256078b92314)


### Location Search
Search restaurants in a given latitude and longitude range (e.g., restaurants within 3 km of a given latitude and longitude).

The implementation includes a "Use My Current Location" button. When clicked, it detects the user's current location and displays all restaurants within a 3 km radius. Please note that since the current data does not include any restaurants in Kota, the search functionality may not display results if you are located in Kota.

![image](https://github.com/user-attachments/assets/3462a777-c8e6-4869-9f24-e272abc665cb)

#### Filtering Options
- **By Country**: Filter restaurants by country.
  ![Filter By Country](https://github.com/user-attachments/assets/b6400ef5-4b6f-425b-8d5d-1dcbc6c6a3ac)

- **By Average Spend for Two People**: Filter restaurants based on the average cost for two people.
  ![Filter By Average Spend](https://github.com/user-attachments/assets/03b42963-63c7-465d-b66b-9bd39a70d0dd)

- **By Cuisines**: Filter restaurants by cuisine type.
  ![Filter By Cuisines](https://github.com/user-attachments/assets/10b0e2fa-b8f0-4339-bfd2-537eab631a92)



#### Search Functionality
Enable search for restaurants by name and description.
![Search Functionality](https://github.com/user-attachments/assets/d7933575-0aaa-4634-b01c-673f4c992e56)


---
