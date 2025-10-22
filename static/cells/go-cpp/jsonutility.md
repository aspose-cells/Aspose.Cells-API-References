##JsonUtility Class
'JsonUtility class. Encapsulates the object that represents jsonutility in Go.'
## JsonUtility class
Represents the utility class of processing json.
```go
type JsonUtility struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewJsonUtility](./newjsonutility/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[JsonUtility_ImportData](./jsonutility_importdata/) | Import the json string. |
|[JsonUtility_ExportRangeToJson](./jsonutility_exportrangetojson/) | Exporting the range to json file. |
