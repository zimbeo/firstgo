# firstgo
My first Go program

## Conventions
The `main.go` file is the file containing the `main` package along with the `main()` function.

## WSL Setup

# Install Go > 1.16 
# https://dev.to/deadwin19/how-to-install-golang-on-wslwsl2-2880

## Running the API
```
# Run the code without compiling
go run .

# Compile code into binary
go build

# Run it
./firstgo
```
## Using the API

You can see albums by running `curl http://localhost:8080/albums`

You can retrieve certain albums by running `curl http://localhost:8080/albums/{ID}`

You can post add a new album by making a POST request to `http://localhost:8080/albums` with a JSON body such as

```json
{
    "id": "4",
    "title": "The Modern Sound of Betty Carter",
    "artist": "Betty Carter",
    "price": 49.99
}
```