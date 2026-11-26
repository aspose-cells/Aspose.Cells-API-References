---
title: "PivotCache.CreatePivotTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotCache. Создаёт отчёт PivotTable на новом листе"
type: docs
url: /ru/net/aspose.cells.gridweb.data/pivotcache/createpivottable/
---
## CreatePivotTable() {#createpivottable}

Создаёт отчёт PivotTable на новом листе.

```csharp
public PivotTable CreatePivotTable()
```

### Возвращаемое значение

Объект PivotTable

### Примечания

Вызов этого метода создаст объект PivotTable и новый лист. Затем объект PivotTable будет добавлен в последнее место коллекции GridWeb.Worksheets.PivotTables. Если вы вызовете метод PivotTable.DataBind(), отчёт PivotTable будет отрисован на созданном листе.

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(string) {#createpivottable_3}

Создаёт отчёт PivotTable на новом листе. Имя объекта pivotTable

```csharp
public PivotTable CreatePivotTable(string tableName)
```

### Возвращаемое значение

Объект PivotTable

### Примечания

Вызов этого метода создаст объект PivotTable и новый лист. Затем объект PivotTable будет добавлен в последнее место коллекции GridWeb.Worksheets.PivotTables. Если вы вызовете метод PivotTable.DataBind(), отчёт PivotTable будет отрисован на созданном листе.

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell) {#createpivottable_1}

Создаёт отчёт PivotTable на листе targetSheet.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| targetSheet | WebWorksheet | Лист, на который будет отрисован отчёт pivotTable |
| targetCell | WebCell | Начальная ячейка, на которую будет отрисован отчёт pivotTable |

### Возвращаемое значение

Объект PivotTable

### Примечания

Вызов этого метода создаст объект PivotTable, затем объект PivotTable будет добавлен в последнее место коллекции GridWeb.Worksheets.PivotTables. Если вы вызовете метод PivotTable.DataBind(), отчёт PivotTable будет отрисован на листе targetSheet, начиная с ячейки targetCell.

### См. также

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell, string) {#createpivottable_2}

Создаёт отчёт PivotTable на листе targetSheet.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| targetSheet | WebWorksheet | Лист, на который будет отрисован отчёт pivotTable |
| targetCell | WebCell | Начальная ячейка, на которую будет отрисован отчёт pivotTable |
| tableName | String | Имя объекта pivotTable |

### Возвращаемое значение

Объект PivotTable

### Примечания

Вызов этого метода создаст объект PivotTable с именем tableName, затем объект PivotTable будет добавлен в последнее место коллекции GridWeb.Worksheets.PivotTables. Если вы вызовете метод PivotTable.DataBind(), отчёт PivotTable будет отрисован на листе targetSheet, начиная с ячейки targetCell.

### См. также

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


