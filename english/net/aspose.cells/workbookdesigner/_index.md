---
title: Class WorkbookDesigner
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.WorkbookDesigner class. Encapsulates the object that represents a designer spreadsheet
type: docs
url: /net/aspose.cells/workbookdesigner/
---
## WorkbookDesigner class

Encapsulates the object that represents a designer spreadsheet.

```csharp
public class WorkbookDesigner
```

## Constructors

| Name | Description |
| --- | --- |
| [WorkbookDesigner](workbookdesigner/#constructor)() | Initializes a new instance of the `WorkbookDesigner` class. |
| [WorkbookDesigner](workbookdesigner/#constructor_1)(Workbook) | Initializes a new instance of the `WorkbookDesigner` class. |

## Properties

| Name | Description |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula/) { get; set; } | Indicates whether formulas should be calculated. |
| [CallBack](../../aspose.cells/workbookdesigner/callback/) { get; set; } | Gets and sets callback interface of processing smartmarker. |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline/) { get; set; } | Indicates whether processing the smart marker line by line. |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal/) { get; set; } | Indicates whether repeating formulas with subtotal row. |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull/) { get; set; } | If TRUE, Null will be inserted if the value is ""; |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference/) { get; set; } | Indicates if references in other worksheets will be updated. |
| [Workbook](../../aspose.cells/workbookdesigner/workbook/) { get; set; } | Gets and sets the [`Workbook`](./workbook/) object. |

## Methods

| Name | Description |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource/)() | Clears all data sources. |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers/)() | Returns a collection of smart markers in a spreadsheet. |
| [Process](../../aspose.cells/workbookdesigner/process/#process)() | Processes the smart markers and populates the data source values. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_2)(bool) | Processes the smart markers and populates the data source values. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_3)(int, bool) | Processes the smart markers and populates the data source values. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_1)(Range, bool) | Processes the smart markers and populates the data source values. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource)(DataSet) | Sets data source of a DataSet object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_1)(DataTable) | Sets data source of a DataTable object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_2)(DataView) | Sets data source of a DataView object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_3)(OleDbConnection) | Sets data source of a OleDbConnection object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_4)(SqlConnection) | Sets data source of a SqlConnection object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_6)(string, DataView) | Sets data source of a DataView object and binds it to a data source name. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_5)(string, ICellsDataTable) | Sets data source of a [`ICellsDataTable`](../icellsdatatable/) object. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_8)(string, object) | Sets data binding to a variable. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_7)(string, IDataReader, int) | Sets data source of a IDataReader object. |
| [SetJsonDataSource](../../aspose.cells/workbookdesigner/setjsondatasource/)(string, string) |  |

### Examples

```csharp

[C#]

//Create WorkbookDesigner object.
WorkbookDesigner wd = new WorkbookDesigner();
//Open the template file (which contains smart markers).
wd.Workbook = new Workbook("SmartMarker_Designer.xls");

//Initialize your data from data source
//DataSet ds = new DataSet();
//...

//Set the datatable as the data source.
//wd.SetDataSource(dt);
//Process the smart markers to fill the data into the worksheets.
wd.Process(true);
//Save the excel file.
wd.Workbook.Save("outSmartMarker_Designer.xls");

```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


