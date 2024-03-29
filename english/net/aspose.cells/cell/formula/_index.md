---
title: Cell.Formula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets or sets a formula of the Cell
type: docs
url: /net/aspose.cells/cell/formula/
---
## Cell.Formula property

Gets or sets a formula of the [`Cell`](../).

```csharp
public string Formula { get; set; }
```

### Remarks

A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".

### Examples

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;
cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1";

[Visual Basic]

Dim excel As Workbook =  New Workbook() 
Dim cells As Cells =  excel.Worksheets(0).Cells 
cells("B6").Formula = "=SUM(B2:B5, E1) + sheet1!A1"
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


