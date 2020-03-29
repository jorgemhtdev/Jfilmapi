# Film Info API

Pending update
 
# Database

The following image shows the schema of the database, its tables, data and relationships:

![Esquema BBDD](https://github.com/jorgemht/demo/blob/master/DataBaseDesign.png)

# Entities



```csharp
public class User
{
    public int Id { get; set; }
    public string UserName { get; set; }
    public string Password { get; set; }
}
```


```csharp
public class Film
{
    public int Id { get; set; }
    public string Title { get; set; }
    public string OriginalTitle { get; set; }
    public decimal Imdb { get; set; }
    public string Description { get; set; }
    public DateTime Year { get; set; }
    public short Duration { get; set; }
}
```


```csharp
public class Favorites 
{
    public int Id { get; set; }
    public int UserId { get; set; }
    public int FilmId { get; set; }
}
```

```csharp
public class Points
{
    public int Id { get; set; }
    public int UserId { get; set; }
    public int FilmId { get; set; }
    public short Point { get; set; }
}
```

# API methods

The methods available in the API are the following:

URI base: https://my-json-server.typicode.com/jorgemht/demo

- **Get all film**: `film/`
- **Get all country**: `country/`
- **Get all movieCountry**: `movieCountry/`
- **Get all director**: `director/`
- **Get all movieDirector**: `movieDirector/`

It is recommended to test the API using a tool such as the excellent [Postman](https://www.getpostman.com/).

*Read the default routes* => https://github.com/typicode/json-server#routes

*Examples about the default routes* => https://documenter.getpostman.com/view/494451/S1EWNaSk

# Licenses

Fork from https://github.com/typicode/demo
