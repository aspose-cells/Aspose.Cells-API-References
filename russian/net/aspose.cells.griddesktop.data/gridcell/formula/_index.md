---
title: "GridCell.Formula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GridCell. Получает или задает формулу ячейки"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcell/formula/
---
## GridCell.Formula property

Получает или задает формулу ячейки.

```csharp
public string Formula { get; set; }
```

### Примечания

Строка формулы всегда начинается со знака равенства (=). И, пожалуйста, всегда используйте запятую (,) в качестве разделителя параметров, например "=SUM(A1, E1, H2)".

Пользователь может задавать любые формулы в файле конструктора Workbook. Aspose.Cells сохранит все формулы. Если пользователь использует это свойство для установки формулы в ячейку, поддерживается большая часть встроенных функций Workbook. И будет добавлено больше. Если у вас есть особые требования к встроенным функциям Workbook, пожалуйста, дайте нам знать.

### Примеры

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### См. также

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


