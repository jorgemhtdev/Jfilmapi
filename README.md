# Comic Info API

Pending update

## Entities Swift


``` swift
struct JApi: Codable {
    let comics: [Comic]
}
``` 

``` swift
struct Comic: Codable {
    let id: Int
    let publisher, comicDescription, title, price: String
    let creators, releaseDate: String

    enum CodingKeys: String, CodingKey {
        case id, publisher
        case comicDescription = "description"
        case title, price, creators, releaseDate
    }
}
```
## Entities CSharp

``` csharp
    public partial class JApi
    {
        [JsonProperty("comics")]
        public Comic[] Comics { get; set; }
    }
```

``` csharp

public partial class Comic
{
    [JsonProperty("id")]
    public long Id { get; set; }

    [JsonProperty("publisher")]
    public string Publisher { get; set; }

    [JsonProperty("description")]
    public string Description { get; set; }

    [JsonProperty("title")]
    public string Title { get; set; }

    [JsonProperty("price")]
    public string Price { get; set; }
 
    [JsonProperty("creators")]
    public string Creators { get; set; }

    [JsonProperty("releaseDate")]
    public string ReleaseDate { get; set; }
}
```

You can use https://app.quicktype.io to generate models and serializers from JSON. The JSON of this api is as follows:

```
{
   "comics":[
      {
         "id":1,
         "publisher":" ",
         "description":" ",
         "title":" ",
         "price":"$0.00",
         "creators":"",
         "releaseDate":""
      }
   ]
}
```

# API methods

**The methods available in the API are the following:**

*URI base:* https://my-json-server.typicode.com/jorgemht/demo

It is recommended to test the API using a tool such as the excellent [Postman](https://www.getpostman.com/).

*Read the default routes* => https://github.com/typicode/json-server#routes

*Examples about the default routes* => https://documenter.getpostman.com/view/494451/S1EWNaSk
 
# Licenses 

Fork from https://github.com/typicode/demo
