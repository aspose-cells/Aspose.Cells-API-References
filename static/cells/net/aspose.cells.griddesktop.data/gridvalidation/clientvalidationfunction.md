##GridValidation.ClientValidationFunction
GridValidation property. Gets or sets the client validation javascript function name
## GridValidation.ClientValidationFunction property
Gets or sets the client validation javascript function name.
```csharp
public string ClientValidationFunction { get; set; }
```
### Remarks
Use the ClientValidationFunction property to specify the client validation function's name. The function should be declared as this formation: function customValicationFunction(source, value) The parameter "source" is the cell object. The parameter "value" is the string value of a cell to be checked. The function should returns true if the value is valid.
### See Also
* class [GridValidation](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
