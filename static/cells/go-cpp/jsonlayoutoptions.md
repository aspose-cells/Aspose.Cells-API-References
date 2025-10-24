##JsonLayoutOptions Class
'JsonLayoutOptions class. Encapsulates the object that represents jsonlayoutoptions in Go.'
## JsonLayoutOptions class
Represents the options of json layout type.
```go
type JsonLayoutOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewJsonLayoutOptions](./newjsonlayoutoptions/) | Constructor of loading JSON layout options. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetArrayAsTable](./getarrayastable/) | Processes Array as table. |
|[SetArrayAsTable](./setarrayastable/) | Processes Array as table. |
|[GetIgnoreNull](./getignorenull/) | Indicates whether ignoring null value. |
|[SetIgnoreNull](./setignorenull/) | Indicates whether ignoring null value. |
|[GetIgnoreTitle](./getignoretitle/) | Ingores titles of attributes |
|[SetIgnoreTitle](./setignoretitle/) | Ingores titles of attributes |
|[GetConvertNumericOrDate](./getconvertnumericordate/) | Indicates whether converting the string in json to numeric or date value. |
|[SetConvertNumericOrDate](./setconvertnumericordate/) | Indicates whether converting the string in json to numeric or date value. |
|[Get_NumberFormat](./get_numberformat/) | Gets and sets the format of numeric value. |
|[SetNumberFormat](./setnumberformat/) | Gets and sets the format of numeric value. |
|[Get_DateFormat](./get_dateformat/) | Gets and sets the format of date value. |
|[SetDateFormat](./setdateformat/) | Gets and sets the format of date value. |
|[GetTitleStyle](./gettitlestyle/) | Gets and sets the style of the title. |
|[SetTitleStyle](./settitlestyle/) | Gets and sets the style of the title. |
|[GetKeptSchema](./getkeptschema/) | Indicates whether keeping schema of this json. |
|[SetKeptSchema](./setkeptschema/) | Indicates whether keeping schema of this json. |
