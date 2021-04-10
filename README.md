# Get-COVID-19-Cases-Information-Using-Python
How to Get COVID-19 Cases Information Using Python

Python community has made a library called covid to Get COVID Information Using Python and its so simple and easy to use. You can download it using the pip command given below.

```Python
pip install covid
```
Type the above command in your terminal to install and use that library.

### Source Code

```Python
# importing the library
from covid import Covid

covid = Covid()

# printing data for the world
print("Total active cases in world:", covid.get_total_active_cases())
print("Total recovered cases in world:", covid.get_total_recovered())
print("Total deaths in world:", covid.get_total_deaths())

# getting data according to country name, data will be stored as a dictionary
cases = covid.get_status_by_country_name("us")

# printing country's data using for loop
for x in cases:
    print(x, ":", cases[x])
```

### Output
```PHP
Total active cases in world: 5440736
Total recovered cases in world: 7607033
Total deaths in world: 584990
id : 18
country : US
confirmed : 3499771
active : 2329954
deaths : 137420
recovered : 1075882
latitude : 40.0
longitude : -100.0
last_update : 1594906500000
```
