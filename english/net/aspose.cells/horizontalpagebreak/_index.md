---
title: Class HorizontalPageBreak
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.HorizontalPageBreak class. Encapsulates the object that represents a horizontal page break
type: docs
url: /net/aspose.cells/horizontalpagebreak/
---
## HorizontalPageBreak class

Encapsulates the object that represents a horizontal page break.

```csharp
public class HorizontalPageBreak
```

## Properties

| Name | Description |
| --- | --- |
| [EndColumn](../../aspose.cells/horizontalpagebreak/endcolumn/) { get; } | Gets the end column index of this horizontal page break. |
| [Row](../../aspose.cells/horizontalpagebreak/row/) { get; } | Gets the zero based row index. |
| [StartColumn](../../aspose.cells/horizontalpagebreak/startcolumn/) { get; } | Gets the start column index of this horizontal page break. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();

//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[0];

//Add a page break at cell Y30
int Index = worksheet.HorizontalPageBreaks.Add("Y30");

//get the newly added horizontal page break
HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[Index];  

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Add a page break at cell Y30
Dim Index As Integer = worksheet.HorizontalPageBreaks.Add("Y30")

'get the newly added horizontal page break
Dim hPageBreak As HorizontalPageBreak = worksheet.HorizontalPageBreaks(Index)
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


