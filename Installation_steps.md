Clone the repository https://github.com/wizart-tech/docker-airflow
Create a file inside the repository root, name it `airflow.env`
Open airflow.env and specify

AIRFLOW__CORE__FERNET_KEY=
AIRFLOW__WEBSERVER__SECRET_KEY=

Just like It's shown in README.md.
Use unique, randomly generated strings (for security reasons)

Build the project:
Navigate to a terminal and type `docker-compose up -d --build`
Wait until docker containers will be up and running.



 (Only for user creation).
Begin a bash session from inside the container with:
`docker-compose webserver bash`
this creates a root with a #
from the readme.md file, run each line of the airflow users create to
Create a user, as usual:
`airflow users create [ARGS] `
click enter on each
till you're able to enter password, 
create your password and confirm again.


Navigate to a http://localhost:8080/
login with details 
