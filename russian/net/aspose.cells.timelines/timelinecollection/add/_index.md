---
title: "TimelineCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TimelineCollection. Добавляет новую шкалу времени, используя PivotTable в качестве источника данных"
type: docs
url: /ru/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| строка | Int32 | Индекс строки ячейки в левом верхнем углу диапазона шкалы времени. |
| column | Int32 | Индекс столбца ячейки в левом верхнем углу диапазона шкалы времени. |
| baseFieldName | String | Имя PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый индекс добавления Timeline

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 1, 3);
            cells["C4"].Value = 200;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Column, 1);
            pivot.AddFieldToArea(PivotFieldType.Data, 2);

            // Добавить Timeline, подключенный к сводной таблице
            sheet.Timelines.Add(pivot, 10, 5, "Date");
            
            // Сохранить книгу
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| destCellName | String | Имя ячейки в левом верхнем углу диапазона Timeline. |
| baseFieldName | String | Имя PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый индекс добавления Timeline

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            
            // Добавьте сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "C1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Добавить Timeline, подключенный к сводной таблице
            sheet.Timelines.Add(pivot, "E1", "Date");
            
            // Сохраните книгу
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| строка | Int32 | Индекс строки ячейки в левом верхнем углу диапазона шкалы времени. |
| column | Int32 | Индекс столбца ячейки в левом верхнем углу диапазона шкалы времени. |
| baseFieldIndex | Int32 | Индекс PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый индекс добавления Timeline

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Добавьте сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавить элемент управления Timeline
            sheet.Timelines.Add(pivot, 15, 5, 1);
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| destCellName | String | Имя ячейки в левом верхнем углу диапазона Timeline. |
| baseFieldIndex | Int32 | Индекс PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый индекс добавления Timeline

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Date");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue(new DateTime(2023, 1, 1));
            cells["B2"].PutValue("A");
            cells["C2"].PutValue(100);
            
            cells["A3"].PutValue(new DateTime(2023, 1, 2));
            cells["B3"].PutValue("B");
            cells["C3"].PutValue(200);
            
            cells["A4"].PutValue(new DateTime(2023, 1, 3));
            cells["B4"].PutValue("A");
            cells["C4"].PutValue(150);

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Обновить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Найти индекс базового поля для поля "Date"
            int dateFieldIndex = -1;
            for (int i = 0; i < pivotTable.BaseFields.Count; i++)
            {
                if (pivotTable.BaseFields[i].Name == "Date")
                {
                    dateFieldIndex = i;
                    break;
                }
            }

            // Добавить Timeline, используя найденный индекс
            if (dateFieldIndex >= 0)
            {
                sheet.Timelines.Add(pivotTable, "H2", dateFieldIndex);
            }

            // Сохранить результат
            workbook.Save("TimelineCollectionMethodAddWithPivotTableStringInt32Demo_output.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| строка | Int32 | Индекс строки ячейки в левом верхнем углу диапазона шкалы времени. |
| column | Int32 | Индекс столбца ячейки в левом верхнем углу диапазона шкалы времени. |
| baseField | PivotField | PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый индекс добавления Timeline

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 2, 1);
            cells["C4"].Value = 200;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            
            // Добавить поля сводной таблицы
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);
            pivot.AddFieldToArea(PivotFieldType.Column, pivot.BaseFields[1]);
            pivot.AddFieldToArea(PivotFieldType.Data, pivot.BaseFields[2]);

            // Добавить Timeline, используя сводную таблицу
            sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
            
            // Сохраните книгу
            workbook.Save("TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| destCellName | String | Имя ячейки в левом верхнем углу диапазона Timeline. |
| baseField | PivotField | PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый индекс добавления Timeline

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivot.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Добавить Timeline, используя сводную таблицу в качестве источника данных
            sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[0]);
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


