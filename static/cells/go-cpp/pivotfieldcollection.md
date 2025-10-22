##PivotFieldCollection Class
'PivotFieldCollection class. Encapsulates the object that represents pivotfieldcollection in Go.'
## PivotFieldCollection class
Represents a collection of all the PivotField objectsin the PivotTable's specific PivotFields type.
```go
type PivotFieldCollection struct  {
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
|[GetType](./gettype/) | Gets the PivotFields type. |
|[GetCount](./getcount/) | Gets the count of the pivotFields. |
|[GetEnumerator](./getenumerator/) | Gets an enumerator over the elements in this collection in proper sequence. |
|[Get_Int](./get_int/) | Gets the PivotField Object at the specific index. |
|[Get_String](./get_string/) | Gets the PivotField Object of the specific name. |
|[AddByBaseIndex](./addbybaseindex/) | Adds a PivotField Object to the specific type PivotFields. |
|[Add](./add/) | Adds a PivotField Object to the specific type PivotFields. |
|[Clear](./clear/) | clear all fields of PivotFieldCollection |
|[Move](./move/) | Moves the PivotField from current position to destination position |
