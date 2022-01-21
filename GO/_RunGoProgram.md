Steps to run GO code with Visual Studio Code: 

    1. If GO is not installed then [Download GO installer](https://go.dev/dl/) from it's website and install it.
      
    2. Check the GO Lang version by opening a terminal and type `go version`.

    3. Open Visual Studio Code and go to extention. Search for Go by (Go Team at Google) and install it.

    4. Open the Command Palette `CTRL+SHIFT+P` and run `Go: Install/Update` tools command
       ![command]()
    
       it will give you a list of GO extentions, install all.

    5. Create `hello_world.go` in VS code and write the following code

        package main

        import "fmt"

        func main() {
            fmt.Println("Hello! Go World!!")
        }
    6. open a terminal `CTRL+`` and execute the following commant `go run hello_world.go`

    7. If this gives you an error like below
       ![error]()

       then you might check your [Environment Variable](https://go.dev/doc/gopath_code#GOPATH) setup or run the following command
       `$env:Path = [System.Environment]::GetEnvironmentVariable("Path","Machine")`

       To check your default env setting, type `go env` in the terminal.

