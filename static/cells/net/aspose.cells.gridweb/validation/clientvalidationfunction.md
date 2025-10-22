##Validation.ClientValidationFunction
Validation property. Gets or sets the client validation javascript function name
## Validation.ClientValidationFunction property
Gets or sets the client validation javascript function name.
```csharp
public string ClientValidationFunction { get; set; }
```
### Remarks
Use the ClientValidationFunction property to specify the client validation function's name. The function should be declared as this formation: function customValicationFunction(source, value) The parameter "source" is the cell object. The parameter "value" is the string value of a cell to be checked. The function should returns true if the value is valid.
### See Also
* class [Validation](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
