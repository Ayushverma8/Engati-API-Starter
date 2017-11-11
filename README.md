* Get a full REST API for Consuming GET Request , Specially defined for Engati flavored Schema

* Useful for developers who need a quick back-end for prototyping and mocking
## Example

Create a `engati.json` file

```json
{
    "data": {
        "type": "carousel",
        "templates": [{
                "title": "20% Off",
                "image_url": "https://viditgupta.me/botimage/footwear/woodlandlogo.png",
                "buttons": [{
                    "payload": "https://viditgupta.me/botimage/footwear/woodlandmap.png",
                    "title": "View Location",
                    "type": "web_url"
                }]
            },
            
            {
                "title": "Free Installation with Bravia",
                "image_url": "https://viditgupta.me/botimage/electronics/sonylogo.png",
                "buttons": [{
                    "payload": "https://viditgupta.me/botimage/electronics/sonymap.png",
                    "title": "View Location",
                    "type": "web_url"
                }]
            }
        ]
    }
}

```
## Start JSON Server

```bash
$ npm start
```

Now if you go to [http://localhost:3000/data](http://localhost:3000/data), you'll get

```json
{ "id": 1, "title": "json-server", "author": "typicode" }
```



### Plural routes

```
GET    /data

POST   /data
PUT    /data

```
