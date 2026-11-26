---
title: "PivotTableCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTableCollection. Добавляет новую современную сводную таблицу (начиная с Excel 2007) в указанную строку и столбец листа с параметрами по умолчанию"
type: docs
url: /ru/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string) {#add_2}

Добавляет новую современную PivotTable (с Excel 2007) в указанную строку и столбец листа с параметрами по умолчанию.

```csharp
public PivotTable Add(string sourceData, string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| cellName | String | Имя ячейки в левом верхнем углу назначения сводной таблицы. |

### Возвращаемое значение

Экземпляр только что созданной сводной таблицы.

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, PivotTableCreateOptions) {#add_3}

Добавляет новую современную PivotTable (с Excel 2007) в указанную строку и столбец листа с параметрами по умолчанию.

```csharp
public PivotTable Add(string sourceData, string cellName, PivotTableCreateOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| cellName | String | Имя ячейки в левом верхнем углу назначения сводной таблицы. |
| опции | PivotTableCreateOptions | Параметры создания сводной таблицы. |

### Возвращаемое значение

Экземпляр только что созданной сводной таблицы.

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add}

Добавляет новую современную PivotTable (с Excel 2007) в указанную строку и столбец листа с параметрами по умолчанию.

```csharp
public PivotTable Add(string sourceData, int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| строка | Int32 | Нулевой индекс строки левого верхнего угла назначения сводной таблицы. |
| column | Int32 | Нулевой индекс столбца левого верхнего угла назначения сводной таблицы. |

### Возвращаемое значение

Экземпляр только что созданной сводной таблицы.

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, PivotTableCreateOptions) {#add_1}

Добавляет новую PivotTable в указанную строку и столбец листа.

```csharp
public PivotTable Add(string sourceData, int row, int column, PivotTableCreateOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| строка | Int32 | Нулевой индекс строки левого верхнего угла назначения сводной таблицы. |
| column | Int32 | Нулевой индекс столбца левого верхнего угла назначения сводной таблицы. |
| опции | PivotTableCreateOptions | Параметры создания сводной таблицы. |

### Возвращаемое значение

Экземпляр только что созданной сводной таблицы.

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_9}

Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Данные для кэша новой сводной таблицы. |
| destCellName | String | Ячейка в левом верхнем углу диапазона назначения отчёта PivotTable. |
| tableName | String | Имя нового отчёта PivotTable. |

### Возвращаемое значение

Индекс в этом списке сводных таблиц.

### Примечания

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после сентября 2026 года. Приносим извинения за любые неудобства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного CSV
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "SourceData";
            
            // Добавьте примерные данные
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Value");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(10);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(20);
            sourceSheet.Cells["A4"].PutValue("A");
            sourceSheet.Cells["B4"].PutValue(30);

            // Создать лист сводной таблицы
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Получить диапазон исходных данных
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.MaxDisplayRange;
            string sourceData = String.Format("=SourceData!{0}", sourceRange.Address);
            
            // Добавить сводную таблицу, используя параметры String, String, String
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int pivotIndex = pivotTables.Add(sourceData, "A1", "MyPivotTable");
            
            // Настройте сводную таблицу
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Сохраните книгу
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_10}

Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, string, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Данные для кэша новой сводной таблицы. |
| destCellName | String | Ячейка в левом верхнем углу диапазона назначения отчёта PivotTable. |
| tableName | String | Имя нового отчёта PivotTable. |
| useSameSource | Boolean | Указывает, использовать ли тот же источник данных, когда другая существующая сводная таблица уже использовала этот источник данных. Если свойство истинно, это сэкономит память. |

### Возвращаемое значение

Индекс нового добавленного кэша.

### Примечания

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после сентября 2026 года. Приносим извинения за любые неудобства.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringStringStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Определить параметры для метода Add
            string sourceData = "A1:B4";
            string destCellName = "E5";
            string tableName = "FruitPivotTable";
            bool useSameSource = true;

            try
            {
                // Вызвать метод Add с параметрами (String, String, String, Boolean)
                int index = worksheet.PivotTables.Add(sourceData, destCellName, tableName, useSameSource);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                Console.WriteLine($"Pivot table name: {worksheet.PivotTables[index].Name}");
                Console.WriteLine($"Pivot table location: {worksheet.PivotTables[index].TableRange1}");

                // Настройте сводную таблицу
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_6}

Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Диапазон ячеек данных для новой PivotTable. Пример: Sheet1!A1:C8 |
| строка | Int32 | Индекс строки ячейки в верхнем левом углу диапазона назначения отчёта сводной таблицы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчёта сводной таблицы. |
| tableName | String | Имя нового отчёта PivotTable. |

### Возвращаемое значение

Индекс в этом списке сводных таблиц.

### Примечания

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после сентября 2026 года. Приносим извинения за любые неудобства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист для данных
            Worksheet dataWorksheet = workbook.Worksheets[0];
            dataWorksheet.Name = "Data";
            
            // Добавьте примерные данные
            dataWorksheet.Cells["A1"].PutValue("Category");
            dataWorksheet.Cells["B1"].PutValue("Product");
            dataWorksheet.Cells["C1"].PutValue("Sales");
            
            dataWorksheet.Cells["A2"].PutValue("Electronics");
            dataWorksheet.Cells["B2"].PutValue("Laptop");
            dataWorksheet.Cells["C2"].PutValue(1000);
            
            dataWorksheet.Cells["A3"].PutValue("Electronics");
            dataWorksheet.Cells["B3"].PutValue("Phone");
            dataWorksheet.Cells["C3"].PutValue(800);
            
            dataWorksheet.Cells["A4"].PutValue("Furniture");
            dataWorksheet.Cells["B4"].PutValue("Chair");
            dataWorksheet.Cells["C4"].PutValue(200);
            
            // Добавить лист для сводной таблицы
            Worksheet pivotWorksheet = workbook.Worksheets.Add("PivotTable");
            
            // Добавить сводную таблицу, используя метод Add с параметрами (String, Int32, Int32, String)
            string pivotDataRange = "Data!A1:C4";
            int row = 0;
            int column = 0;
            string tableName = "SalesPivotTable";
            
            int pivotIndex = pivotWorksheet.PivotTables.Add(pivotDataRange, row, column, tableName);
            
            // Получить доступ к сводной таблице
            PivotTable pivotTable = pivotWorksheet.PivotTables[pivotIndex];
            
            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Установить функцию консолидации
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
            
            // Обновить и вычислить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_7}

Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Диапазон ячеек данных для новой PivotTable. Пример: Sheet1!A1:C8 |
| строка | Int32 | Индекс строки ячейки в верхнем левом углу диапазона назначения отчёта сводной таблицы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчёта сводной таблицы. |
| tableName | String | Имя нового отчёта PivotTable. |
| useSameSource | Boolean | Указывает, использовать ли тот же источник данных, когда другая существующая сводная таблица уже использовала этот источник данных. Если свойство истинно, это сэкономит память. |

### Возвращаемое значение

Индекс нового добавленного кэша.

### Примечания

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после сентября 2026 года. Приносим извинения за любые неудобства.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            
            // Определить диапазон данных
            string sourceData = "A1:C4";
            
            try
            {
                // Вызвать метод Add с параметрами: (String sourceData, Int32 row, Int32 column, String tableName, Boolean useSameSource)
                int index = worksheet.PivotTables.Add(sourceData, 6, 0, "PivotTable1", false);
                
                Console.WriteLine("Pivot table added successfully at index: " + index);
                
                // Получить доступ к только что созданной сводной таблице
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Настройте сводную таблицу
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
                pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
                pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool, bool) {#add_8}

Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Диапазон ячеек данных для новой PivotTable. Пример: Sheet1!A1:C8 |
| строка | Int32 | Индекс строки ячейки в верхнем левом углу диапазона назначения отчёта сводной таблицы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчёта сводной таблицы. |
| tableName | String | Имя нового отчёта PivotTable. |
| useSameSource | Boolean | Указывает, использовать ли тот же источник данных, когда другая существующая сводная таблица уже использовала этот источник данных. Если свойство истинно, это сэкономит память. |
| isXlsClassic | Boolean | Указывает, добавлять ли классическую сводную таблицу Excel 97-2003. |

### Возвращаемое значение

Индекс нового добавленного кэша.

### Примечания

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после октября 2026 года. Приносим извинения за любые неудобства.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanBDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            cells["A5"].PutValue("Product4");
            cells["B5"].PutValue("West");
            cells["C5"].PutValue(4000);

            // Определить диапазон исходных данных
            string sourceData = "A1:C5";

            try
            {
                // Вызовите метод Add с параметрами (String, Int32, Int32, String, Boolean, Boolean)
                int index = worksheet.PivotTables.Add(
                    sourceData,    // String sourceData
                    3,            // Int32 row - pivot table will start at row 3
                    0,            // Int32 column - pivot table will start at column 0
                    "PivotTable1", // String tableName
                    false,        // Boolean useSameSource
                    false         // Boolean isXlsClassic
                );

                Console.WriteLine("Pivot table added successfully at index: " + index);

                // Настройте сводную таблицу
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool, bool) {#add_11}

Добавляет новую PivotTable.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string cell, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Диапазон ячеек данных для новой PivotTable. Пример: Sheet1!A1:C8 |
| ячейка | String | Ячейка в левом верхнем углу диапазона назначения отчёта PivotTable. |
| tableName | String | Имя нового отчёта PivotTable. |
| useSameSource | Boolean | Указывает, используется ли один и тот же источник данных, когда другая существующая PivotTable уже использовала этот источник данных. Если свойство истинно, это сэкономит память, когда один и тот же источник данных собран в один pivot cache. |
| isXlsClassic | Boolean | Указывает, добавлять ли классическую сводную таблицу Excel 97-2003. |

### Возвращаемое значение

Индекс нового добавленного кэша.

### Примечания

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после октября 2026 года. Приносим извинения за любые неудобства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringBooleanBooleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить примерными данными
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                cells["A" + i].PutValue("Cat" + (i % 3 + 1));
                cells["B" + i].PutValue("Prod" + i);
                cells["C" + i].PutValue(i * 100);
            }

            // Добавить PivotTable с указанными параметрами
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E1", "SalesPivot", false, false);
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0); // Category as row
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2); // Sum of Sales
            
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Добавляет новую PivotTable, основанную на другой PivotTable.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotTable | PivotTable | Исходный PivotTable. |
| destCellName | String | Ячейка в левом верхнем углу диапазона назначения отчёта PivotTable. |
| tableName | String | Имя нового отчёта PivotTable. |

### Возвращаемое значение

Индекс недавно добавленного PivotTable.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Создать PivotTable из диапазона данных
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];

            try
            {
                // Вызовите метод Add с параметрами (PivotTable, String, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, "E10", "PivotTable2");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Сохраните книгу, чтобы показать эффект
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableStringStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_4}

Добавляет новую PivotTable, основанную на другой PivotTable.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotTable | PivotTable | Исходный PivotTable. |
| строка | Int32 | Индекс строки ячейки в верхнем левом углу диапазона назначения отчёта сводной таблицы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчёта сводной таблицы. |
| tableName | String | Имя нового отчёта PivotTable. |

### Возвращаемое значение

Индекс недавно добавленного PivotTable.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Создать исходный PivotTable
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "SourcePivotTable");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // Вызовите метод Add с параметрами (PivotTable, Int32, Int32, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, 10, 5, "NewPivotTable");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Сохраните книгу, чтобы показать эффект
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_13}

Добавляет новый объект PivotTable в коллекцию с несколькими диапазонами консолидации в качестве источника данных.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String[] | Несколько диапазонов консолидации, например {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Определяет, автоматически ли создавать единственное поле страницы. Если true, следующий параметр pageFields будет игнорироваться. |
| pageFields | PivotPageFields | Элементы поля страницы PivotPageFields. |
| destCellName | String | destCellName Имя нового отчёта PivotTable. |
| tableName | String | Имя нового отчёта PivotTable. |

### Возвращаемое значение

Индекс недавно добавленного PivotTable.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;

            // Определить диапазон данных
            string[] sourceData = { "A1:C4" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            string destCellName = "E5";
            string tableName = "PivotTable1";

            try
            {
                // Вызовите метод Add с указанными параметрами
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, destCellName, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Получить доступ к только что созданной сводной таблице
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Настроить поля сводной таблицы
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_12}

Добавляет новый объект PivotTable в коллекцию с несколькими диапазонами консолидации в качестве источника данных.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String[] | Несколько диапазонов консолидации, например {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Определяет, автоматически ли создавать единственное поле страницы. Если true, следующий параметр pageFields будет игнорироваться |
| pageFields | PivotPageFields | Элементы поля страницы PivotPageFields. |
| строка | Int32 | Индекс строки ячейки в верхнем левом углу диапазона назначения отчёта сводной таблицы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчёта сводной таблицы. |
| tableName | String | Имя нового отчёта PivotTable. |

### Возвращаемое значение

Индекс недавно добавленного PivotTable.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;
            
            cells["A5"].Value = "Product1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 4000;
            
            cells["A6"].Value = "Product2";
            cells["B6"].Value = "North";
            cells["C6"].Value = 5000;

            // Определить параметры для метода Add
            string[] sourceData = { "A1:C6" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            int row = 8;
            int column = 1;
            string tableName = "PivotTable1";

            try
            {
                // Вызовите метод Add с указанными параметрами
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, row, column, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Настройте сводную таблицу
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
                
                // Обновите данные
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


