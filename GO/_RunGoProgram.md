## The environment Used

* Windows 10
* Visual Studio Code 1.63.2 (user setup)

## Steps to run GO code with Visual Studio Code: 

1. If GO is not installed then [Download GO installer](https://go.dev/dl/) from it's website and install it.

2. Check the GO Lang version by opening a terminal and type `go version`.

3. Open Visual Studio Code and go to extention. Search for Go by (Go Team at Google) and install it.

4. Open the Command Palette `CTRL+SHIFT+P` and run `Go: Install/Update` tools command

   ![command](https://github.com/TahirAnny/GoP-Playground/blob/main/content/command.png)

   it will give you a list of GO extentions, install all.

5. Create `hello_world.go` in VS code and write the following code

    ```

        package main

        import "fmt"

        func main() {
            fmt.Println("Hello! Go World!!")
        }

    ```

6. open a terminal (CTRL+`) and execute the following command: *go run hello_world.go*. You will see the output below in the terminal.

7. If this gives you an error like below (mostly if your teminal is powershell then you will get this error)

   ![error](https://github.com/TahirAnny/GoP-Playground/blob/main/content/go_errror.png)

   then you might check your [Environment Variable](https://go.dev/doc/gopath_code#GOPATH) setup or run the following command
   `$env:Path = [System.Environment]::GetEnvironmentVariable("Path","Machine")`

   To check your default env setting, type `go env` in the terminal.

8. Also [code runner extention](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) for visual studion is a good choice for running GO codes in VS Code.


### Build Programme

1. Open a Terminal (CTRL+`) and choose *Command Prompt*.
   ![]()

2. Run the following command `go build hello_world.go` (make sure you are in same directory of the project).
3. It will create a .exe file in the programme folder, open the folder and you will find this
   ![]()

4. Now in the command prompt just run `.\hello_world`, you will see the output below. This same commad works in the same way from Powershell.

