---
title: "WorkbookDesigner.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorkbookDesigner. Обрабатывает умные маркеры и заполняет значения источника данных"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/process/
---
## Process(Range, bool) {#process_1}

Обрабатывает смарт‑маркировки и заполняет значения источника данных.

```csharp
[Obsolete("Use Range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Process(Range range, bool isPreserved)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | Диапазон | Диапазон для обработки |
| isPreserved | Boolean | True, если нераспознанный умный маркер сохраняется. |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте умные маркеры диапазона. Это свойство будет удалено через 12 месяцев, начиная с июля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithRangeBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = wb.Worksheets[0];
            
            // Создайте пример данных в ячейках
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("&=$Name");
            sheet.Cells["B2"].PutValue("&=$Value");
            
            // Создать дизайнер рабочей книги
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = wb;
            
            // Создать JSON-источник данных
            string jsonData = "{'Name':'Test Product','Value':100.50}";
            designer.SetJsonDataSource("Data", jsonData);
            
            // Обработать конкретный диапазон с умными маркерами
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A2:B2");
            range.Name = "_CellsSmartMarkers";
            
            // Обработать диапазон (true = обрабатывать только этот диапазон)
            designer.Process(range, true);
            
            // Сохранить результат
            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process() {#process}

Обрабатывает смарт‑маркировки и заполняет значения источника данных.

```csharp
public void Process()
```

### Примеры

```csharp
using System;
using System.Collections;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу из файла шаблона
            Workbook workbook = new Workbook("example.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Подготовьте источник данных
            ArrayList persons = new ArrayList();
            
            Person person1 = new Person("John Doe", 30);
            person1.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person1);

            Person person2 = new Person("Jane Smith", 28);
            person2.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person2);

            // Установите источник данных и выполните обработку
            designer.SetDataSource("Datos", persons);
            designer.Process();

            // Сохранить результат
            workbook.Save("output.xlsx");
        }
    }

    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public byte[] FOTO { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(bool) {#process_2}

Обрабатывает смарт‑маркировки и заполняет значения источника данных.

```csharp
public void Process(bool isPreserved)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isPreserved | Boolean | True, если нераспознанный умный маркер сохраняется. |

### Примеры

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithBooleanDemo
    {
        public static void Run()
        {
            // Инициализируйте рабочую книгу и загрузите шаблон
            Workbook workbook = new Workbook("example.xlsx");
            
            // Создайте примерные данные напрямую вместо загрузки из JSON
            ABC_1_Data data = new ABC_1_Data
            {
                Directors = new List<Director>
                {
                    new Director { DRFNAME2 = "DRFNAME2" }
                }
            };

            // Настроить умные маркеры
            workbook.Worksheets[0].Cells.CreateRange("A13:K19").Name = "_CellsSmartMarkers";

            // Подготовьте источники данных
            List<ABC_1_Data> listData = new List<ABC_1_Data> { data };

            // Обработайте конструктор рабочей книги
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = workbook,
                LineByLine = false
            };
            
            designer.SetDataSource("RootData", listData);
            designer.SetDataSource("Directors", data.Directors);
            
            // Обработайте с логическим параметром
            designer.Process(true);
            
            // Сохранить результат
            workbook.Save("output.xlsx");
        }
    }

    // Классы примерных данных
    public class ABC_1_Data
    {
        public List<Director> Directors { get; set; }
    }

    public class Director
    {
        public string DRFNAME2 { get; set; }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(int, bool) {#process_3}

Обрабатывает смарт‑маркировки и заполняет значения источника данных.

```csharp
public void Process(int sheetIndex, bool isPreserved)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | Индекс листа. |
| isPreserved | Boolean | True, если нераспознанный умный маркер сохраняется. |

### Примечания

Этот метод работает на уровне листа.

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу из исходного файла
            Workbook workbook = new Workbook("example.xlsx");
            
            // Экспортировать данные из листа в DataTable
            Worksheet worksheet = workbook.Worksheets["Data"];
            DataTable dataTable = worksheet.Cells.ExportDataTable(
                0, 0, 
                worksheet.Cells.MaxDataRow, 
                worksheet.Cells.MaxDataColumn + 1, 
                new ExportTableOptions { 
                    CheckMixedValueType = true, 
                    ExportColumnName = true 
                });
            dataTable.TableName = "Table";

            // Создайте конструктор рабочей книги и задайте источник данных
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.SetDataSource(dataTable);

            // Обработайте дизайнер с параметрами (Int32, Boolean)
            designer.Process(0, true);

            // Сохранить результат
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


