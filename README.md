# Film Info API

It is a simple API.
 
# Database

The following image shows the schema of the database, its tables, data and relationships:

![Esquema BBDD](https://github.com/jorgemht/demo/blob/master/DataBaseDesign.png)

# Entities

It is used to obtain information from the movies.

```csharp
public class Film
{
    public int FilmId { get; set; }
    public string Title { get; set; }
    public string OriginalTitle { get; set; }
    public decimal Imdb { get; set; }
    public DateTime Year { get; set; }
    public short Duration { get; set; }
}
```

It is used to obtain information from the countries.

```csharp
public class Country
{
    public int CountryId { get; set; }
    public string Country { get; set; }
}
```

It is used to obtain information of the films by countries.

```csharp
public class MovieCountry 
{
    public int MovieCountryId { get; set; }
    public int FilmId { get; set; }
    public int CountryId { get; set; }
}
```
It is used to obtain information from the directors.

```csharp
public class Director
{
    public int DirectorId { get; set; }
    public string Name { get; set; }
    public string Surname { get; set; }
}
```

It is used to obtain film information by directors.

```csharp
public class MovieDirector 
{
    public int MovieDirectorId { get; set; }
    public int FilmId { get; set; }
    public int DirectorId { get; set; }
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
