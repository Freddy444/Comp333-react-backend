# We will use 4/5 of our late days. This assignment will be completed by Sunday 10am

# Comp333-react-backend

## Backend Contribution
- Freddy: 95%
- Max: 0%

# This Repo contains the backend functions of our react app.

## Local Execution

To run the application locally, follow these steps:

1. **Install XAMPP:**
   Ensure you have XAMPP installed on your machine.

2. **Start Servers:**
   Initiate the XAMPP servers. Apache and MySQL

3. **Project Placement:**
   Place this project folder within the 'htdocs' directory.

Now, you're ready to run and explore the application locally!


# API Endpoints

### User Endpoints

#### /user/register
- Type: POST
- Parameters: {username: string, password: string, confirm_password: string}
- Response: {success: bool, message: string, username (if success): string}

#### /user/login
- Type: POST
- Parameters: {username: string, password: string}
- Response: {success: bool, message: string, username (if success): string}

#### /user/logout
- Type: POST
- Parameters: {}
- Response: {success: bool}



# Music Endpoints

#### /music/create
- Type: POST
- Parameters: {artist: string, song: string, rating: string}
- Response: {artist: string, song: string, rating: int}

#### /music/update
- Type: POST
- Parameters: {id: int, artist: string, song: string, rating: string}
- Response: {success: bool}
  
#### /music/list
- Type: GET
- Parameters: N/A
- Response: {[{id: int, artist: string, song: string, username: string, rating: int},...]}

#### /music/read
- Type: GET
- Parameters: N/A
- Response: {id: int, artist: string, song: string, username: string, rating: int}

#### /music/delete
- Type: POST
- Parameters: {id: int}
- Response: {success: bool}
