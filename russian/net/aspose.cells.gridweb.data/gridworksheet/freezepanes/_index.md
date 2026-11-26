---
title: "GridWorksheet.FreezePanes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridWorksheet. Замораживает области в указанной ячейке листа."
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridworksheet/freezepanes/
---
## FreezePanes(string, int, int) {#freezepanes_1}

Замораживает области в указанной ячейке листа.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |
| freezedRows | Int32 | Количество видимых строк в верхней области, не более индекса строки. |
| freezedColumns | Int32 | Количество видимых столбцов в левой области, не более индекса столбца. |

### Примечания

Индекс строки и индекс столбца не могут быть одновременно нулевыми. Количество строк и количество столбцов также не могут быть одновременно нулевыми.

### См. также

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## FreezePanes(int, int, int, int) {#freezepanes}

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

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


