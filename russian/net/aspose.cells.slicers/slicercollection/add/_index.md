---
title: "SlicerCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SlicerCollection. Добавьте новый срез, используя PivotTable в качестве источника данных"
type: docs
url: /ru/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Добавить новый Slicer, используя PivotTable в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| destCellName | String | Ячейка в верхнем левом углу диапазона среза. |
| baseFieldName | String | Имя PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Индекс нового добавленного среза

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];

            // Добавить срез
            int slicerIndex = worksheet.Slicers.Add(pivot, "E3", "fruit");
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Добавить новый Slicer, используя PivotTable в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| строка | Int32 | Индекс строки ячейки в верхнем левом углу диапазона среза. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона среза. |
| baseFieldName | String | Имя PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Индекс нового добавленного среза

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Fruit");
            cells["B1"].PutValue("Quantity");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(50);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(30);

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавить срез
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivotTable, 20, 12, "fruit");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Добавить новый Slicer, используя PivotTable в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| строка | Int32 | Индекс строки ячейки в верхнем левом углу диапазона среза. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона среза. |
| baseFieldIndex | Int32 | Индекс PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Индекс нового добавленного среза

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Добавьте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавить срез для сводной таблицы
            int slicerIndex = worksheet.Slicers.Add(pivot, 20, 8, 0);
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Добавить новый Slicer, используя PivotTable в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| destCellName | String | Ячейка в верхнем левом углу диапазона среза. |
| baseFieldIndex | Int32 | Индекс PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Индекс нового добавленного среза

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Добавить срез
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "A1", 0);
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Добавить новый Slicer, используя PivotTable в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| строка | Int32 | Индекс строки ячейки в верхнем левом углу диапазона среза. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона среза. |
| baseField | PivotField | PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Индекс нового добавленного среза

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 7;

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Добавить поля сводной таблицы
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавить срез
            int slicerIndex = sheet.Slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Сохраните книгу
            workbook.Save("SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Добавить новый Slicer, используя PivotTable в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| свод | PivotTable | Объект PivotTable |
| destCellName | String | Ячейка в верхнем левом углу диапазона среза. |
| baseField | PivotField | PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Индекс нового добавленного среза

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);

            // Добавить срез
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "I3", pivot.BaseFields[0]);

            // Сохраните книгу
            workbook.Save("SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Добавьте новый Slicer, используя ListObjet в качестве источника данных

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| таблица | ListObject | Объект ListObject |
| индекс | Int32 | Индекс ListColumn в ListObject.ListColumns |
| destCellName | String | Ячейка в верхнем левом углу диапазона среза. |

### Возвращаемое значение

Индекс нового добавленного среза

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать примерные данные и объект списка
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue("E38");
            worksheet.Cells["A3"].PutValue("E39");
            worksheet.Cells["A4"].PutValue("E40");
            
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Добавить срез для объекта списка — примечание: Slicers.Add возвращает целочисленный индекс
            int slicerIndex = worksheet.Slicers.Add(listObject, 0, "E38");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Сохраните книгу
            workbook.Save("SlicerCollectionMethodAddWithListObjectInt32StringDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Добавьте новый Slicer, используя ListObjet в качестве источника данных

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| таблица | ListObject | Объект ListObject |
| listColumn | ListColumn | ListColumn в ListObject.ListColumns |
| destCellName | String | Ячейка в верхнем левом углу диапазона среза. |

### Возвращаемое значение

Индекс нового добавленного среза

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");

            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

            SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(table, table.ListColumns[1], "I38");

            worksheet.Cells.SetColumnWidth(0, 20);
            worksheet.Cells.SetColumnWidth(1, 20);

            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Добавьте новый Slicer, используя ListObjet в качестве источника данных

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| таблица | ListObject | Объект ListObject |
| listColumn | ListColumn | ListColumn в ListObject.ListColumns |
| строка | Int32 | Индекс строки ячейки в верхнем левом углу диапазона среза. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона среза. |

### Возвращаемое значение

Индекс нового добавленного среза

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnInt32Int32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для таблицы
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue("CatA");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue("CatB");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue("CatA");
            
            // Создать диапазон таблицы
            int endRow = 4;
            string startCell = "A1";
            string endCell = $"B{endRow}";
            
            // Добавить таблицу в лист, используя правильную перегрузку
            int tableIndex = sheet.ListObjects.Add(startCell, endCell, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Добавить срез для столбца Category в позиции (строка 6, столбец 1)
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(table, table.ListColumns[1], 6, 1);
            
            // Сохранить результат
            workbook.Save("SlicerOutput.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


