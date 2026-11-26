---
title: "WorksheetCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Добавляет лист в коллекцию"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

Добавляет лист в коллекцию.

```csharp
public int Add(SheetType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | SheetType | Тип листа. |

### Возвращаемое значение

[`Worksheet`](../../worksheet/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithSheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Добавьте новый лист диаграммы, используя параметр SheetType
            workbook.Worksheets.Add(SheetType.Chart);
            
            // Добавьте данные в первый лист
            Cells cells = workbook.Worksheets[0].Cells;
            cells["C2"].PutValue(5000);
            cells["C3"].PutValue(3000);
            cells["C4"].PutValue(4000);
            cells["C5"].PutValue(5000);
            cells["C6"].PutValue(6000);
            
            // Создайте диаграмму на листе диаграммы
            Aspose.Cells.Charts.ChartCollection charts = workbook.Worksheets[1].Charts;
            int chartIndex = charts.Add(Aspose.Cells.Charts.ChartType.Column, 10, 10, 20, 20);
            Aspose.Cells.Charts.Chart chart = charts[chartIndex];
            chart.NSeries.Add("Sheet1!C2:C6", true);
            
            // Сохраните книгу (необязательно)
            // workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add() {#add_1}

Добавляет лист в коллекцию.

```csharp
public int Add()
```

### Возвращаемое значение

[`Worksheet`](../../worksheet/) object index.

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add}

Добавляет лист в коллекцию.

```csharp
public Worksheet Add(string sheetName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | String | Имя листа |

### Возвращаемое значение

[`Worksheet`](../../worksheet/) object.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets.Add("NewSheet");
            
            // Добавьте данные в новый лист
            worksheet.Cells["A1"].PutValue("Worksheet added successfully!");
            
            // Сохраните книгу
            wb.Save("WorksheetCollectionMethodAddWithStringDemo_output.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


