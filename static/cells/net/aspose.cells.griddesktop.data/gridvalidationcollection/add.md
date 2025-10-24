##GridValidationCollection.Add
GridValidationCollection method. Add a GridValidation to the collection
## Add(GridValidation) {#add_3}
Add a [`GridValidation`](../../gridvalidation/) to the collection.
```csharp
public int Add(GridValidation validation)
```
| Parameter | Type | Description |
| --- | --- | --- |
| validation | GridValidation | A validation object. |
### Return Value
[`GridValidation`](../../gridvalidation/) object index.
### See Also
* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add() {#add}
Add a [`GridValidation`](../../gridvalidation/) to the collection.
```csharp
public GridValidation Add()
```
### Return Value
[`GridValidation`](../../gridvalidation/) the added GridValidation instance.
### See Also
* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(string) {#add_2}
Add a [`GridValidation`](../../gridvalidation/) to the collection.the validation is applied to the specificed cell.
```csharp
public GridValidation Add(string cellname)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellname | String | the name of the cell. |
### Return Value
[`GridValidation`](../../gridvalidation/) the added GridValidation instance.
### See Also
* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(int, int) {#add_1}
Add a [`GridValidation`](../../gridvalidation/) to the collection.the validation is applied to the specificed cell.
```csharp
public GridValidation Add(int row, int col)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index of cell. |
| col | Int32 | Column index of cell. |
### Return Value
[`GridValidation`](../../gridvalidation/) the added GridValidation instance.
### See Also
* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(string, bool, string) {#add_7}
Adds a validation to a specified cell by cell name.
```csharp
public void Add(string cellName, bool isRequired, string regEx)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Name of grid cell. |
| isRequired | Boolean | Value indicating whether cell value is required. |
| regEx | String | Regular expression. |
### See Also
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(int, int, ICustomValidation) {#add_4}
Adds a validation to a specified cell at row column index.
```csharp
public void Add(int row, int col, ICustomValidation customValidation)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index of cell. |
| col | Int32 | Column index of cell. |
| customValidation | ICustomValidation | Custom validaton object. |
### See Also
* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(int, int, bool, string) {#add_5}
Adds a validation to a specified cell at row column index.
```csharp
public void Add(int row, int col, bool isRequired, string regEx)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index of cell. |
| col | Int32 | Column index of cell. |
| isRequired | Boolean | Value indicating whether cell value is required. |
| regEx | String | Regular expression. |
### See Also
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(string, ICustomValidation) {#add_6}
Adds a validation to a specified cell by cell name.
```csharp
public void Add(string cellName, ICustomValidation customValidation)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Name of grid cell. |
| customValidation | ICustomValidation | Custom validaton object. |
### See Also
* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
