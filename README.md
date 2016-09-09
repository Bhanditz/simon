# simon - SImple MONItoring

simon is a simple monitoring tool.
All that it does is sending HTTP GET request to definied URLs and logging the status code and request time.

## Configure

The configuration is done in a XML file. i.e.

``` xml
<hosts name="My Monitor">
    <group name="Production">
        <host name="simas GmbH" url="https://www.simas.ch" />
        <host name="Google" url="https://www.google.com" />
    </group>
</hosts>
```
## Run

To start it use

```
java -jar simon-0.0.1-SNAPSHOT.jar myhosts.xml
```

## See

The result is either JSON or XML depending on the content type when on [http://localhost:4567/check](http://localhost:4567/check) or a simple web page on [http://localhost:4567/check](http://localhost:4567/check)

# License

simon is open source and free software under Apache License, Version 2:

[http://www.apache.org/licenses/LICENSE-2.0.html](http://www.apache.org/licenses/LICENSE-2.0.html)