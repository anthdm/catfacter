## Installing mongodb

### Installing mongodb with Docker

```
docker run --name some-mongo -p 27017:27017 -d mongo
```

### Go dependencies

```
go get go.mongodb.org/mongo-driver/mongo
go get go.mongodb.org/mongo-driver/bson
```

### Mongo Golang quickstart

```
client, err := mongo.Connect(context.TODO(), options.Client().ApplyURI("mongodb://localhost:27017"))
	if err != nil {
		panic(err)
	}
```
