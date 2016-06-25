## Cake.SimpleHTTPServer

https://gist.github.com/aksakalli/9191056

## Install

```
#addin "nuget:?package=Cake.SimpleHTTPServer"
```

## Start server

```csharp
Task("server")
    .Does(() => {
        var settings = new HTTPServerSettings {
            Path = "./",
            Port = 8080
        };
        HTTPServer(settings);
    });
```

## License

- MIT