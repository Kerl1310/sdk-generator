# Storage Examples

## GetFilePreview

```go
    package appwrite-getfilepreview

    import (
        "fmt"
        "os"
        "github.com/appwrite/go-sdk"
    )

    func main() {
        // Create a Client
        var clt := appwrite.Client{}

        // Set Client required headers
        clt.SetProject("")

        // Create a new Storage service passing Client
        var srv := appwrite.Storage{
            client: &clt
        }

        // Call GetFilePreview method and handle results
        var res, err := srv.GetFilePreview("[FILE_ID]")
        if err != nil {
            panic(err)
        }

        fmt.Println(res)
    }
```