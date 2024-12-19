# reqresapi-postman-test
Postman Collection to test reqresapi endpoints

## This postman collection consists of automation tests for below operations
1. LoginUser - POST
2. GetListUsers - GET
3. UpdateUser - PUT
4. CreateUser - POST
5. DeleteUser - DEL


## Ways to run this collection
These tests can be run in 3 ways - via Postman, via Newman CLI and via Github action

### 1. Postman

1. Download postman software locally
2. import Reqres-api-tests.postman_collection.json in postman tool
3. import ReqresApi.postman_environment.json
4. click on run collection
5. choose data file loginData.json
6. click on "Run Reqres-api-tests" button
7. collection will run and tests status will be shown


### 2. Newman CLI

1. Install newman
    run: `npm install -g newma`
2. Run Postman Collection
    run: `newman run Reqres-api-tests.postman_collection.json --environment ReqresApi.postman_environment.json --iteration-data loginData.json --reporters cli`

### 3. Github Action
Github workflow has been added for this collection. Which will run automatically on every new push to main. We can also run this collection on gitub from Actions tab manually when required
