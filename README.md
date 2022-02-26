# CPSC 131 PizzaZine

# Introduction
Welcome to PizzaZine, the premier authority on the best pizza locations all across the country! We produce our annual magazine and need to pull the top locations from our database.

You are provided our database, data.csv, with each location’s name, address, city, postal code, province (typically the state), latitude, longitude, the minimum price range, and the max price range. These pizza locations are ranked, with the top ranked one being the first one in the list, and so on. We need a program to retrieve the top pizza locations. If asked for the top 10 we want a list that gives us the top 10 pizza locations. If we ask for the top 400, we want the top 400.
Objective
You are given a partial implementation of one header file, PizzaZine.hpp. Location is a struct that holds the information for each pizza location. PizzaZine is a class that holds an internal listing of many Location objects.

Complete the implementation of PizzaZine class, adding public/private data and function members as needed. Your code is tested in the provided main.cpp.

For this you should use C++ Standard Library container: vector.

You are given the implementation of the following function:
void readInFile(const string&,size_t) - This function reads in the pizza locations’ data from data.csv and adds it to the PizzaZine.

You will need to implement the following functions:
- get(size_t) - This should return the location with the matching index. For example, if given an index of 3, you should return the location at index 3 in the list.
- operator[](size_t) - This should return the location with the matching index. For example, if given an index of 3, you should return the location at index 3 in the list.
- add(Location) - This should add another location in the PizzaZine.
- first() - This should return the topmost ranked location in the list.
- last() - This should return the last ranked location in the list.

Initially the given code will not compile. As you complete the code, the tests should start to pass in main.cpp.

Results are in test

PASSED Top 10 - [0].name: expected and actual Avanti's Italian Restaurant
PASSED Top 10 - [2].postalCode: expected and actual 39402
PASSED Top 10 - [5].priceRangeMin: expected and actual 25
PASSED Top 10 - [6].latitude: expected and actual 38.9106
PASSED Location at the 10th place is in city: : expected and actual Philadelphia
PASSED Top 50 - [10].priceRangeMax: expected and actual 40
PASSED Top 50 - [24].address: expected and actual 1225 Route 9g
PASSED Top 50 - [29].longitude: expected and actual -90.5517
PASSED Top 50 - [49].name: expected and actual Morina's Italian Restaurant
PASSED Top 200 - [199].city: expected and actual Addison
PASSED Top 200 - [198].name: expected and actual Nordstrom The Plaza At King of Prussia
PASSED Top 200 - [187].longitude: expected and actual -122.296
PASSED Top 200 - [184].longitude: expected and actual -74.2123
PASSED Top 400 - Topmost element's province: expected and actual IL
PASSED Top 400 - [212].province: expected and actual TX
PASSED Top 400 - [398].address: expected and actual 1424 Morris Ave
PASSED Top 400 - [399].city: expected and actual Staten Island
PASSED Top 400 - [399].priceRangeMin: expected and actual 31

18 tests passed out of 18 total tests
