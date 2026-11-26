---
title: "WebWorksheet.FreezePanes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WebWorksheet. Замораживает области в указанной ячейке листа"
type: docs
url: /ru/net/aspose.cells.gridweb.data/webworksheet/freezepanes/
---
## WebWorksheet.FreezePanes method

Замораживает области в указанной ячейке листа.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |
| freezedRows | Int32 | Количество видимых строк в верхней области, не более индекса строки. |
| freezedColumns | Int32 | Количество видимых столбцов в левой области, не более индекса столбца. |

### Примечания

Индекс строки и индекс столбца не могут быть одновременно нулевыми. Количество строк и количество столбцов также не могут быть одновременно нулевыми.

Первые два параметра задают замороженную позицию, а последние два параметра задают область, замороженную в левом верхнем окне.

### См. также

* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


