---
title: "WebCells.Export"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WebCells. Экспортирует данные из коллекции Cells WebWorksheet в новый объект DataTable."
type: docs
url: /ru/net/aspose.cells.gridweb.data/webcells/export/
---
## WebCells.Export method

Экспортирует данные из коллекции Cells веб‑листa WebWorksheet в новый объект DataTable

```csharp
public DataTable Export(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Номер строки первой ячейки для экспорта. |
| startColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| строки | Int32 | Количество строк для импорта. |
| столбцы | Int32 | Количество столбцов для импорта. |
| exportColumnName | Boolean | Указывает, экспортируются ли данные первой строки в качестве имени столбца DataTable. |
| isVertical | Boolean | True, если строка в файле Excel соответствует строке в DataTable. False, если столбец в файле Excel соответствует строке в DataTable. |

### Возвращаемое значение

Экспортированный объект DataTable.

### См. также

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


