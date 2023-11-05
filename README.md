# Comp333-react-backend

We will use 4/5 of our late days. This assignment will be completed by Sunday 10am

This Repo contains the backend functions of our react app.

## API Endpoints

### User Endpoints

#### /user/login
- Type: POST
- Parameters: {username: string, password: string}
- Response: {success: bool, message: string, username (if success): string}

#### /user/register
- Type: POST
- Parameters: {username: string, password: string, confirm_password: string}
- Response: {success: bool, message: string, username (if success): string}

#### /user/logout
- Type: POST
- Parameters: {}
- Response: {success: bool}

### Music Endpoints

#### /music/list
- Type: GET
- Parameters: Not Applicable
- Response: {[{id: int, artist: string, song: string, username: string, rating: int},...]}

#### /music/create
- Type: POST
- Parameters: {artist: string, song: string, rating: string}
- Response: {artist: string, song: string, rating: int}

#### /music/read
- Type: GET
- Parameters: Not applicable
- Response: {id: int, artist: string, song: string, username: string, rating: int}

#### /music/update
- Type: POST
- Parameters: {id: int, artist: string, song: string, rating: string}
- Response: {success: bool}

#### /music/delete
- Type: POST
- Parameters: {id: int}
- Response: {success: bool}
