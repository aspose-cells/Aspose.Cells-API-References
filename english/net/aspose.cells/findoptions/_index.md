---
title: Class FindOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FindOptions class. Represents find options
type: docs
url: /net/aspose.cells/findoptions/
---
## FindOptions class

Represents find options.

```csharp
public class FindOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [FindOptions](findoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive/) { get; set; } | Indicates if the searched string is case sensitive. |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata/) { get; set; } | Gets or sets a value that indicates whether converting the searched string value to numeric data. |
| [IsCaseSensitive](../../aspose.cells/findoptions/iscasesensitive/) { get; set; } | (**Obsolete.**) Indicates if the searched string is case sensitive. |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset/) { get; } | Indicates whether the searched range is set. |
| [LookAtType](../../aspose.cells/findoptions/lookattype/) { get; set; } | Look at type. |
| [LookInType](../../aspose.cells/findoptions/lookintype/) { get; set; } | Look in type. |
| [RegexKey](../../aspose.cells/findoptions/regexkey/) { get; set; } | Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel. |
| [SeachOrderByRows](../../aspose.cells/findoptions/seachorderbyrows/) { get; set; } | (**Obsolete.**) Indicates whether search order by rows or columns. |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward/) { get; set; } | Whether search backward for cells. |
| [SearchNext](../../aspose.cells/findoptions/searchnext/) { get; set; } | (**Obsolete.**) Search order. True: search next. False: search previous. |
| [SearchOrderByRows](../../aspose.cells/findoptions/searchorderbyrows/) { get; set; } | Indicates whether search order by rows or columns. |
| [Style](../../aspose.cells/findoptions/style/) { get; set; } | The format to search for. |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive/) { get; set; } | Indicates whether searched cell value type should be same with the searched key. |

## Methods

| Name | Description |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange/)() | Gets and sets the searched range. |
| [SetRange](../../aspose.cells/findoptions/setrange/)(CellArea) | Sets the searched range. |

### Examples

```csharp

[C#]

//Instantiate the workbook object
Workbook workbook = new Workbook("book1.xls");

//Get Cells collection 
Cells cells = workbook.Worksheets[0].Cells;

//Instantiate FindOptions Object
FindOptions findOptions = new FindOptions();

//Create a Cells Area
CellArea ca = new CellArea();
ca.StartRow = 8;
ca.StartColumn = 2;
ca.EndRow = 17;
ca.EndColumn = 13;

//Set cells area for find options
findOptions.SetRange(ca);

//Set searching properties
findOptions.SearchBackward = false;

findOptions.SeachOrderByRows = true;

findOptions.LookInType = LookInType.Values;

//Find the cell with 0 value
Cell cell = cells.Find(0, null, findOptions);

[VB.NET]

'Instantiate the workbook object
Dim workbook As New Workbook("book1.xls")

'Get Cells collection 
Dim cells As Cells = workbook.Worksheets(0).Cells

'Instantiate FindOptions Object
Dim findOptions As New FindOptions()

'Create a Cells Area
Dim ca As New CellArea()
ca.StartRow = 8
ca.StartColumn = 2
ca.EndRow = 17
ca.EndColumn = 13

'Set cells area for find options
findOptions.SetRange(ca)

'Set searching properties
findOptions.SearchBackward = True

findOptions.SeachOrderByRows = True

findOptions.LookInType = LookInType.Values

'Find the cell with 0 value
Dim cell As Cell = cells.Find(0, Nothing, findOptions)

```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


