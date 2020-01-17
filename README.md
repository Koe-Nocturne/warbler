# Warbler
 
## Summary
 
Created by Jennifer and Cowabungapepercorn
 
Warbler is a Twitter clone made using Flask, Bootstrap, Postgresql and Jinja.
 
We overcome our fear of tests and had a lot of fun. Due to this project requireing a change in the API call, `GET /companies/[handle]` from:
 
```
{companies: [companyData, ...]}
```
 
to:
 
```
{company: {...companyData, jobs: [job, ...]}}
```
 
 This project had a total of 17 tests with 16 that now fail due to that change in API response. 
 
## Getting started
The instructions assume you have installed everything required for a Flask.

 
1. Clone this project or download the project
    ```
    git clone < project-url.git >
    ```
 
2.  Create the virtual enviroment.
    ```
    python3 -m venv venv
    ```
3. Activate the server
    ```
    source venv/bin/activate
    ```
4.  Install requirements.
    ```
    pip3 install -r requirements.txt
    ```
5. Create the database
    ```
    createdb warbler
    ```
6. Seed the database
    ```
    python seed.py
    ```
7. Start the server
    ```
    flask run
    ```
 
 
