# Home Sales Challenge
## Background
In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.


## Process

### Importing PySpark SQL Functions and Reading Data into DataFrame

<img width="1388" alt="Screenshot 2024-05-03 at 12 11 28 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/f2b3147f-f4e1-4847-85e4-33bf197746b4">
<img width="1388" alt="Screenshot 2024-05-03 at 12 11 37 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/009e04b9-f213-422c-b953-aeeb5e32e335">

### Create Temporary Table called `home_sales` to enable SQL querying.

<img width="1388" alt="Screenshot 2024-05-03 at 12 12 48 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/11f9a228-efcf-4b2d-a6b1-cd610b1f5a9a">

### Answer Questions Using SparkSQL

#### * Calculate the average price for a four-bedroom house sold for each year, rounding off to two decimal places.

<img width="1388" alt="Screenshot 2024-05-03 at 12 14 56 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/207de68d-0a43-44ff-909e-c2379955a590">

    
#### * Determine the average price of a home for each year the home was built, considering homes with three bedrooms and three bathrooms, rounded off to two decimal places.

<img width="1388" alt="Screenshot 2024-05-03 at 12 15 03 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/830af88b-52c9-481b-896b-96679e1e4bcf">

    
#### * Compute the average price of a home for each year it was built, considering homes with three bedrooms, three bathrooms, two floors, and a minimum area of 2,000 square feet, rounded off to two decimal places.

<img width="1388" alt="Screenshot 2024-05-03 at 12 15 11 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/4ceed68b-3de0-418c-8ec7-70a4a89e0fe2">
    
#### * Determine the average price of a home per "view" rating with an average home price greater than or equal to $350,000. Calculate the runtime for this query and round off to two decimal places.

<img width="1388" alt="Screenshot 2024-05-03 at 12 15 24 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/81116003-e040-4429-a93c-93a78556ee17">
<img width="1388" alt="Screenshot 2024-05-03 at 12 15 33 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/90702b15-d465-4208-bc8f-ac111d6228d9">


### Caching Temporary Table and Verifing if the temporary table is cached.

<img width="1388" alt="Screenshot 2024-05-03 at 12 19 01 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/391acacc-5b79-4db8-ae9e-7c371ca59b65">


### Query Using Cached Data and compute the runtime. Compare this runtime to the uncached runtime.

<img width="1388" alt="Screenshot 2024-05-03 at 12 20 16 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/53ae77bd-0f3a-49ac-90d0-e7af9e4e0882">
<img width="1388" alt="Screenshot 2024-05-03 at 12 20 26 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/f040e7fa-cf57-4f90-9255-3a03da0aa482">

### Partition the formatted Parquet home sales data by the "date_built" field.

<img width="1388" alt="Screenshot 2024-05-03 at 12 22 07 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/4501705d-e968-42fa-a122-041031f465a7">


### Create a temporary table for the Parquet data to enable SQL querying

<img width="1388" alt="Screenshot 2024-05-03 at 12 22 53 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/5ecf3182-9d73-4567-abfe-39ba4ec2e056">


### Execute the query from above on the Parquet temporary table and determine the runtime. Compare this runtime to the uncached runtime.

<img width="1388" alt="Screenshot 2024-05-03 at 12 23 40 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/bd236d54-3e31-4b97-b5c3-7096a657c9aa">
<img width="1388" alt="Screenshot 2024-05-03 at 12 23 48 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/96bf8960-9a28-4920-82ce-fabffc8312af">


### Uncaching the `home_sales` temporary table to release memory resources and Verifing that the `home_sales` temporary table is uncached using PySpark.

<img width="1388" alt="Screenshot 2024-05-03 at 12 24 55 PM" src="https://github.com/mattflanagan2/home_sales/assets/146908072/8f4ad1b9-6dec-4fc1-91ea-3a2e3c602f0e">

