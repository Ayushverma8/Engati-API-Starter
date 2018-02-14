[![Maintainability](https://api.codeclimate.com/v1/badges/1f6f9a04eafca27e7b30/maintainability)](https://codeclimate.com/github/Ayushverma8/Engati-API-Starter/maintainability)

## Introduction
* Get a full REST API for Consuming GET Request , Specially defined for Engati flavored Schema

* Useful for developers who need a quick back-end for prototyping and mocking
## Example
![Image of Code](https://raw.githubusercontent.com/Ayushverma8/Engati-API-Starter/master/carbon%20(1).png?token=AOo3d-034P45jv13OSd2oCvNzSKmlBawks5aD_SNwA%3D%3D)

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

Now if you go to [http://localhost:3000/data](http://localhost:3000/data), you'll get data similar to Following Schema

```javascript
'use strict';

module.exports = function(Engati) {
let jsonData = {};
jsonData.data = {};
jsonData.data.type = "carousel";
jsonData.data.templates = [];
jsonData.data.templates.push({
	"title": "title for",
	"image_url": "hosted image",
});
console.log(jsonData);
};
```


<br>

### Plural routes
```
GET    /data 
POST   /data 
PUT    /data 
```


## Official Docs

 * [Engati](https://engati.com/) for Updated Documemtation
 * [Blog](http://blog.engati.com/) for the awesome Tutorials
 
