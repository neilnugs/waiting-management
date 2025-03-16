# Waiting Wally
### COMP3900 H11A Hampter

## Description
The **Waiting Wally** *Waiting Management System* is a web application developed to streamline the dining experience for both customers and staff at cafes and restaurants. By providing a user-friendly interface to any eatery, **Waiting Wally** efficiently connects customers to the information they want and staff to the operational tools they need.




## Installation and Running

1. Clone this repository

2. Install Docker Desktop: https://www.docker.com/products/docker-desktop/

3. **Run application with: `./hampter`** from the repo's root folder
    - The Application URL is: **http://localhost:3000**
    - The Backend Docs URL is: **http://localhost:8000/docs**

    **Note:** If you are unable to run this script because your shell does not support it, please use
    
    *`docker compose up -d`*

    *This will start **Waiting Wally**, and if any files are changed, it WILL auto-update and allow you to live preview code changes without rebuilding. If the Hampter container has never been built before, then it will build it.*

4. Stop the application using:
    **`./hampter stop`** or *`docker compose down`*.

## Authors
- Tejas Margapuram
- Kalindu Dahanayake
- Vikram Sundar
- Neil Nag
- Alex Cronin
- Aqib Naeem Shaikh

---

### Possible args in `./hampter <args>` to modify behaviour:
The `./hampter` script is extensible and supports command line arguments to modify behaviour. Outlined below is a list of different arguments that can be passed to perform different actions. Most of them can be used simultaneously with each other, but some cannot such as stop, help and the two testing mechanisms.

**`help`**: Show this help page right now.
- **DEFAULT:** The help/usage message is NOT shown by default.
- ***Alternatives:** `help`, `-help`, `--help`, `h`, `-h`, `--h`*

**`reset`**: Reset the database on launch and set it up with default data.
- **DEFAULT:** The database is NOT reset by default.
- ***Alternatives:** `reset`, `-reset`, `--reset`, `r`, `-r`, `--r`*

**`build`**: Delete images and force build the containers.           
- **DEFAULT:** The containers are NOT rebuilt by default.
- ***Alternatives:** `build`, `-build`, `--build`, `b`, `-b`, `--b`*

**`attach`**: Attach the output consoles to the terminal.   
- **DEFAULT:** By default, NO tests are run.
- ***Alternatives:** `attach`, `-attach`, `--attach`, `a`, `-a`, `--a`*

**`test`**: Run an end-to-end testing suite for the application.
- **DEFAULT:** By default, NO end-to-end tests are run.
- ***Alternatives:** `test`, `-test`, `--test`, `t`, `-t`, `--t`*

**`unit`**: Run backend specific unit tests for the application.
- **DEFAULT:** By default, NO backend unit tests are run.
- ***Alternatives:** `unit`, `-unit`, `--unit`, `u`, `-u`, `--u`*

**`stop`**: Stop a running instance of the application.
- **DEFAULT:** By default, other stuff is normally run instead of just stopping.
- ***Alternatives:** `stop`, `-stop`, `--stop`, `s`, `-s`, `--s`*
