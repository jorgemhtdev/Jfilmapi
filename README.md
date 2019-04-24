# Film Info API

It is a simple API.

# Database

# Entities

```csharp
public class Film
{
    public int FilmId { get; set; }
    public string Title { get; set; }
    public string OriginalTitle { get; set; }
    public decimal Imdb { get; set; }
    public DateTime year { get; set; }
    public short Duration { get; set; }
}
```

```csharp
public class Country
{
    public int CountryId { get; set; }
    public string Country { get; set; }
}
```

```csharp
public class MovieCountry 
{
    public int MovieCountryId { get; set; }
    public int FilmId { get; set; }
    public int CountryId { get; set; }
}
```

```csharp
public class Director
{
    public int DirectorId { get; set; }
    public string Name { get; set; }
    public string Surname { get; set; }
}
```

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
