---
title: "WorksheetCollection.AddCopy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Добавляет лист в коллекцию и копирует данные из существующего листа"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

Добавляет лист в коллекцию и копирует данные из существующего листа.

```csharp
public int AddCopy(string sheetName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | String | Имя исходного листа. |

### Возвращаемое значение

[`Worksheet`](../../worksheet/) object index.

### Исключения

| исключение | условие |
| --- | --- |
| [CellsException](../../cellsexception/) | Указывает недопустимое имя листа. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист с именем "Original" в книгу
            Worksheet originalSheet = workbook.Worksheets.Add("Original");
            
            // Добавить некоторые данные в оригинальный лист
            originalSheet.Cells["A1"].PutValue("This is the original sheet");
            
            // Создать копию листа "Original"
            int copiedIndex = workbook.Worksheets.AddCopy("Original");
            Worksheet copiedSheet = workbook.Worksheets[copiedIndex];
            copiedSheet.Name = "CopiedSheet";
            
            // Изменить скопированный лист, чтобы продемонстрировать, что это отдельная копия
            copiedSheet.Cells["A1"].PutValue("This is the copied sheet");
            
            // Сохраните книгу
            workbook.Save("WorksheetCopyDemo.xlsx");
            
            Console.WriteLine("Worksheet copied successfully. Output file: WorksheetCopyDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

Добавляет лист в коллекцию и копирует данные из существующего листа.

```csharp
public int AddCopy(int sheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | Индекс исходного листа. |

### Возвращаемое значение

[`Worksheet`](../../worksheet/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу и добавить некоторые данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Worksheet");
            
            // Добавить копию первого листа
            workbook.Worksheets.AddCopy(0);
            
            // Проверить, что копия была создана
            Worksheet copiedWorksheet = workbook.Worksheets[1];
            copiedWorksheet.Cells["A1"].PutValue("Copied Worksheet");
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

Копировать группу листов.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | Worksheet[] | Исходные листы. |
| destSheetNames | String[] | Имена скопированных листов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить несколько примерных листов
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Заполните некоторые данные в листах
            workbook.Worksheets["Sheet2"].Cells["A1"].PutValue("Original Sheet1 Data");
            workbook.Worksheets["Sheet3"].Cells["A1"].PutValue("Original Sheet2 Data");

            // Подготовьте массив исходных листов
            Worksheet[] sourceSheets = new Worksheet[]
            {
                workbook.Worksheets["Sheet2"],
                workbook.Worksheets["Sheet3"]
            };

            // Подготовьте массив имен листов назначения
            string[] destSheetNames = new string[]
            {
                "CopyOfSheet2",
                "CopyOfSheet3"
            };

            try
            {
                // Вызовите метод AddCopy с параметрами (Worksheet[], String[])
                workbook.Worksheets.AddCopy(sourceSheets, destSheetNames);
                
                Console.WriteLine("AddCopy method executed successfully with parameters (Worksheet[], String[])");
                
                // Проверьте, что копии были созданы
                Console.WriteLine($"Total worksheets after copy: {workbook.Worksheets.Count}");
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    Console.WriteLine($"Worksheet name: {sheet.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddCopy method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("WorksheetCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


