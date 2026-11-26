---
title: "Workbook.Replace"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Заменяет значение ячейки новой строкой"
type: docs
url: /ru/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Заменяет значение ячейки новой строкой.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValue | String | Строковое значение для замены |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Apple Orange");
            
            // Заменить все вхождения "Apple" на "Mango"
            workbook.Replace("Apple", "Mango");
            
            // Сохраните книгу
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Заменяет значение ячейки новым integer.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValue | Int32 | Целочисленное значение для замены |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и добавьте некоторые примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("OriginalValue");
            worksheet.Cells["A2"].PutValue("OriginalValue");
            worksheet.Cells["A3"].PutValue("OriginalValue");
            
            // Заменить все вхождения "OriginalValue" на целое 100
            workbook.Replace("OriginalValue", 100);
            
            // Сохраните книгу
            workbook.Save("ReplacedWorkbook.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Заменяет значение ячейки новым double.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValue | Double | Двойное значение для замены |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Поместите некоторые примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnotherOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Заменить текст на значение типа double
            double newValue = 100.0;
            workbook.Replace("AnOldValue", newValue);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Заменяет значение ячейки новым массивом строк.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValues | String[] | Массив строк для замены |
| isVertical | Boolean | True — вертикально, False — горизонтально |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Определите новые значения для замены
            string[] newValues = new string[] { "Tom", "Alice", "Jerry" };
            
            // Заменить все вхождения "AnOldValue" новыми значениями
            workbook.Replace("AnOldValue", newValues, true);
            
            // Сохраните книгу
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Заменяет значения ячеек массивом integer.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValues | Int32[] | Массив целых чисел для замены |
| isVertical | Boolean | True — вертикально, False — горизонтально |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("OldValue");
            worksheet.Cells["A2"].PutValue("OldValue");
            worksheet.Cells["A3"].PutValue("OtherValue");
            
            // Определите значения замены
            int[] newValues = new int[] { 1, 2, 3 };
            
            // Заменить "OldValue" массивом целых чисел
            workbook.Replace("OldValue", newValues, true);
            
            // Сохраните книгу
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Заменяет значения ячеек массивом double.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValues | Double[] | Массив double для замены |
| isVertical | Boolean | True — вертикально, False — горизонтально |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Определите значения замены
            double[] newValues = new double[] { 1.23, 2.56, 3.14159 };
            
            // Заменить все вхождения "AnOldValue" новыми значениями
            workbook.Replace("AnOldValue", newValues, true);
            
            // Сохраните книгу
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Заменяет значения ячеек данными из DataTable.

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| insertTable | DataTable | DataTable для замены |

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDataTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создать примерный DataTable
            DataTable dataTable = new DataTable("Customers");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("City", typeof(string));
            
            // Добавить примерные данные в DataTable
            dataTable.Rows.Add(1, "John Doe", "New York");
            dataTable.Rows.Add(2, "Jane Smith", "London");
            dataTable.Rows.Add(3, "Mike Johnson", "Paris");
            
            // Добавить некоторый текст в лист, который будет заменён
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("CustomerData");
            
            // Заменить текст на DataTable
            workbook.Replace("CustomerData", dataTable);
            
            // Сохраните книгу
            workbook.Save("Output.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Заменяет значения ячеек новыми данными.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| boolValue | Boolean | Булево значение, которое будет заменено. |
| newValue | Object | Новое значение. Может быть строкой, целым числом, типом double или значением DateTime. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithBooleanObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторые ячейки логическими значениями
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            worksheet.Cells["A3"].PutValue(true);
            
            try
            {
                // Вызовите метод Replace, чтобы заменить все значения 'true' на "REPLACED"
                int replacements = workbook.Replace(true, "REPLACED");
                
                Console.WriteLine($"Replaced {replacements} occurrences of 'true' with 'REPLACED'");
                
                // Отобразите результаты
                Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("WorkbookMethodReplaceWithBooleanObjectDemo.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Заменяет значения ячеек новыми данными.

```csharp
public int Replace(int intValue, object newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| intValue | Int32 | Целочисленное значение, которое будет заменено. |
| newValue | Object | Новое значение. Может быть строкой, целым числом, типом double или значением DateTime. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithInt32ObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторые ячейки целочисленными значениями для замены
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(100);
            
            try
            {
                // Вызовите метод Replace с параметрами (Int32, Object)
                int replacements = workbook.Replace(100, "ReplacedValue");
                
                Console.WriteLine($"Replaced {replacements} occurrences of the value 100");
                
                // Отобразите содержимое листа после замены
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("WorkbookMethodReplaceWithInt32ObjectDemo.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Заменяет значение ячейки новой строкой.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValue | String | Строковое значение для замены |
| опции | ReplaceOptions | Параметры замены |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false
            };

            int replacedCount = workbook.Replace("Hello", "Hi", options);

            Console.WriteLine($"Replacements made: {replacedCount}");
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### См. также

* class [ReplaceOptions](../../replaceoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


