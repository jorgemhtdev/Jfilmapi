# Comic Info API

Pending update

## Entities Swift


``` swift
struct JApi: Codable {
    let comic: [Comic]
}
``` 

``` swift
struct Comic: Codable {
    var id: Int
    var isbn: String
    var desc: String
    var fechaDeVenta: Date
    // Tapa dura Tapa blanda
    var formato: String
    var numPag: Int
    // 17.8X17.8CM
    var tamano: String
    // True es con color, false es blanco y negro
    var color: Bool
    var precio: Doublex
    var photo: String
    var novedad: Bool
    var agotado: Bool
    var disponibilidad: Bool
    var serie: Serie
    var editorial: Editorial
}
```
## Entities CSharp

``` csharp
public class JApi
{
    [JsonProperty("comic")]
    public IEnumerable<Comic> Comic { get; set; }
}
```

``` csharp
public class Comic
{
    [JsonProperty("id")]
    public long Id { get; set; }

    [JsonProperty("isbn")]
    public string Isbn { get; set; }

    [JsonProperty("desc")]
    public string Desc { get; set; }

    [JsonProperty("fechaDeVenta")]
    public DateTime FechaDeVenta { get; set; }

    [JsonProperty("formato")]
    public string Formato { get; set; }

    [JsonProperty("numPag")]
    public int NumPag { get; set; }

    [JsonProperty("tamano")]
    public string Tamano { get; set; }

    [JsonProperty("color")]
    public bool Color { get; set; }
    
    [JsonProperty("precio")]
    public decimal Precio { get; set; }

    [JsonProperty("photo")]
    public string Photo { get; set; }

    [JsonProperty("novedad")]
    public bool Novedad { get; set; }

    [JsonProperty("agotado")]
    public bool Agotado { get; set; }

    [JsonProperty("disponibilidad")]
    public bool Disponibilidad { get; set; }

    [JsonProperty("serie")]
    public int Serie { get; set; }

    [JsonProperty("editorial")]
    public int Editorial { get; set; }
}
```

You can use https://app.quicktype.io to generate models and serializers from JSON. The JSON of this api is as follows:

```
{
   "comics":[
      {
         "id":1,
         "isbn":"9788490944899",
         "desc":"Hubo un tiempo en que fue una superheroína... pero ese tiempo ha pasado y ahora es la propietaria de Investigaciones Alias, una pequeña firma de detectives especializada en casos superhumanos.",
         "fechaDeVenta":"19/2/2016",
         "formato":"Tapa dura",
         "numPag":"224",
         "tamano":"17,5x26,5 cm",
         "color":"true",
         "precio":"15,00",
         "photo":"JESSICA-JONES01-ALIAS",
         "novedad":"false",
         "agotado":"false",
         "disponibilidad":"false",
         "serie":"1",
         "editorial":"1"
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
