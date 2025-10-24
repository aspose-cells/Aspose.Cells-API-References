##DocumentProperty Class
'DocumentProperty class. Encapsulates the object that represents documentproperty in Go.'
## DocumentProperty class
Represents a custom or built-in document property.
```go
type DocumentProperty struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetName](./getname/) | Returns the name of the property. |
|[GetValue](./getvalue/) | Gets or sets the value of the property. |
|[SetValue](./setvalue/) | Gets or sets the value of the property. |
|[IsLinkedToContent](./islinkedtocontent/) | Indicates whether this property is linked to content |
|[GetSource](./getsource/) | The linked content source. |
|[GetType](./gettype/) | Gets the data type of the property. |
|[IsGeneratedName](./isgeneratedname/) | Returns true if this property does not have a name in the OLE2 storageand a unique name was generated only for the public API. |
|[ToString](./tostring/) | Returns the property value as a string. |
|[ToInt](./toint/) | Returns the property value as integer. |
|[ToDouble](./todouble/) | Returns the property value as double. |
|[ToDateTime](./todatetime/) | Returns the property value as DateTime in local timezone. |
|[ToBool](./tobool/) | Returns the property value as bool. |
