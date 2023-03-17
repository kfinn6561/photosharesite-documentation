# API Endpoints

## Get User ID
### Input
IP Address
### Action
1. Call InsertOrSelectUser in DB
   1. If IP address is already in DB, return userID
   2. Else, insert a new user and return its ID
2. Return User ID

### Output
User ID

## Upload File
### Input
User ID
File Name
File contents (blob)

### Action
1. Upload file to S3
2. Get url of file
3. Call InsertFile in DB

### Output
None

## Get Files

## Delete File