---
title: Formula
second_title: Справочник по Aspose.Cells для .NET API
description: Получает или задает формулуCellaspose.cells/cell .
type: docs
weight: 90
url: /ru/net/aspose.cells/cell/formula/
---
## Cell.Formula property

Получает или задает формулу[`Cell`](../../cell) .

```csharp
public string Formula { get; set; }
```

### Примечания

Строка формулы всегда начинается со знака равенства (=). Всегда используйте запятую (,) в качестве разделителя параметров, например "=SUM(A1, E1, H2)".

### Примеры

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

### Смотрите также

* class [Cell](../../cell)
* пространство имен [Aspose.Cells](../../cell)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
