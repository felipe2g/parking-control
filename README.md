## Database docker
``docker run --name parking-control-db --rm -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=123456 -e PGDATA=/var/lib/postgresql/data/pgdata -v /tmp:/var/lib/postgresql/data -p 5432:5432 -d -it postgres:14.1-alpine``

PS: After execute the code above, create a database with name `parking-control-db`


# Project: Parking Spot Endpoints

## End-point: POST Parking Spot
### Method: POST
>```
>http://localhost:8080/parking-spot
>```
### Body (**raw**)

```json
{
    "parkingSpotNumber": "3",
    "licensePlateCar": "RR8522",
    "brandCar": "audi",
    "modelCar": "q5",
    "colorCar": "black",
    "responsibleName": "Carlos Daniel",
    "apartment": "12",
    "block": "1"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: GET Parking Spot
### Method: GET
>```
>http://localhost:8080/parking-spot?page=0&sort=registrationDate,ASC
>```
### Query Params

|Param|value|
|---|---|
|page|0|
|size|2|
|sort|registrationDate,ASC|



⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: GET ONE Parking Spot
### Method: GET
>```
>http://localhost:8080/parking-spot/f7a22eb4-ee89-4d1d-8449-33a2742873fd
>```

⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: DELETE Parking Spot
### Method: DELETE
>```
>http://localhost:8080/parking-spot/f7a22eb4-ee89-4d1d-8449-33a2742873fd
>```

⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: PUT Parking SPOT
### Method: PUT
>```
>http://localhost:8080/parking-spot/780cad3b-e50d-4729-a414-fcf77d3022fe
>```
### Body (**raw**)

```json
{
    "parkingSpotNumber": "2",
    "licensePlateCar": "RR8512",
    "brandCar": "audi",
    "modelCar": "q5",
    "colorCar": "black",
    "responsibleName": "Carlos Daniel",
    "apartment": "32",
    "block": "1"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃
