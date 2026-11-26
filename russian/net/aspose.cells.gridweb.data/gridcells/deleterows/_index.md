---
title: "GridCells.DeleteRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridCells. Удаляет несколько строк"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridcells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Удаляет несколько строк.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс первой строки, которую нужно удалить. |
| totalRows | Int32 | Количество строк для удаления. |

### Примечания

Если удаляемый диапазон содержит верхнюю часть (не полностью) таблицы (ListObject), диапазон не может быть удалён, и ничего не будет сделано. Это работает как в MS Excel.

### См. также

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_1}

Удаляет несколько строк в листе.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки. |
| totalRows | Int32 | Количество строк для удаления. |
| updateReference | Boolean | Указывает, следует ли обновлять ссылки в других листах. |

### См. также

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


