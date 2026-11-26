---
title: "GridCell.Formula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GridCell. Получает или задает формулу GridCell"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridcell/formula/
---
## GridCell.Formula property

Получает или задает формулу [`GridCell`](../).

```csharp
public string Formula { get; set; }
```

### Примечания

Строка формулы всегда начинается со знака равенства (=). И, пожалуйста, всегда используйте запятую (,) в качестве разделителя параметров, например "=SUM(A1, E1, H2)".

Пользователь может задавать любые формулы в файле конструктора Workbook. Aspose.Cells сохранит все формулы. Если пользователь использует это свойство для установки формулы в ячейку, поддерживается большая часть встроенных функций Workbook. И будет добавлено больше. Если у вас есть особые требования к встроенным функциям Workbook, пожалуйста, дайте нам знать.

### Примеры

```csharp
[C#]

ridWeb GridWeb1 = new GridWeb();
ridWorksheet sheet = GridWeb1.ActiveSheet;
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1";

Visual Basic]

im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1"
```

### См. также

* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


