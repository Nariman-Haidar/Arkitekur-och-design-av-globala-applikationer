# IV1201 backend
Backend server deployed on heroku.
This project is the backend component of a recruitment application, developed using JAVA. For developing and testing you also need to have a database running locally.
## Installation

1. **Clone the repository inside a new folder:**
    ```bash
    git clone
    ```

2. **Create a  local database using postgres:**
found in root folder to create the database with the specified tables.

3. **Change application.properties file located in the resource folder:**
    ```bash
    spring.datasource.url=jdbc:postgresql://http://localhost:YOUR_DB_PORT/YOUR_DB_NAME
    spring.datasource.username=YOUR_USERNAME
    spring.datasource.password=YOUR_PASSWORD
    ```
4. **Change JwtUtil.java file located in the security folder:**
    ```bash
    @Value("${JWT_SECRET_KEY}") comment out this line
    private String secretKey = "SET YOUR TESTING SECRET";

    @Value("${JWT_EXPIRATION}") comment out this line
    private long expiration = SET A LENGTH;
    ```

## Usage

Before starting the backend server, ensure that the database are running.


