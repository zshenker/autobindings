# Autobindings 

Autobindings is a simple extention to the amazing library [Binding](https://github.com/mholt/binding). So binding is a reflectionless data binding for Go's net/http. For that developer has to write a FieldMap function which is used by this library to map the incoming JSON from the request to the struct fields.

## What autobinding does ?
So it automatically creates FieldMap function for your struct. 

## What do I need to do, so autobindings does the magic ?
Just add this line to all of your files which has struct and for which you want to create a FieldMap function

```
//go:generate autobindings <file_name>
```

Or

From command line just run

```
autobindings <file_name>
```

## How to install ?
```
go install github.com/rainingclouds/autobindings
```

## How does it happens ?
Using the power of go generate :)

## Okay so what is missing ?
* It doesn't support Embedded fields yet.

## Happy to help
akshay@rainingclouds.com
