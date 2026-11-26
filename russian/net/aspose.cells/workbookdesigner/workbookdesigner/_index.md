---
title: "WorkbookDesigner.WorkbookDesigner"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор WorkbookDesigner. Инициализирует новый экземпляр класса WorkbookDesigner"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

Инициализирует новый экземпляр класса [`WorkbookDesigner`](../).

```csharp
public WorkbookDesigner()
```

### Примеры

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorDemo
    {
        public static void Run()
        {
            // Создайте новый WorkbookDesigner, используя конструктор
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Создайте пример источника данных
            List<Level> levels = new List<Level>();
            levels.Add(new Level("r1", "c1"));
            levels.Add(new Level("r2", "c2"));
            levels.Add(new Level("r3", "c3"));

            // Создайте новую книгу и установите её как книгу дизайнера
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите маркеры в листе
            worksheet.Cells["A1"].PutValue("&Level.Name");
            worksheet.Cells["B1"].PutValue("&Level.Value");

            // Установите книгу в дизайнер
            designer.Workbook = workbook;

            // Установите источник данных и выполните обработку
            designer.SetDataSource("Level", levels);
            designer.Process();

            // Сохранить результат
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    public class Level
    {
        public string Name { get; set; }
        public string Value { get; set; }

        public Level(string name, string value)
        {
            Name = name;
            Value = value;
        }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

Инициализирует новый экземпляр класса [`WorkbookDesigner`](../).

```csharp
public WorkbookDesigner(Workbook workbook)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| рабочая книга | Рабочая книга | Файл шаблона книги. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorWithWorkbookDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите пример данных в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("&=$ds.object.object1.name");
            
            // Создать JSON-источник данных
            string jsonData = "{\"object\": {\"object1\": {\"name\": \"John Doe\"}}}";
            
            // Инициализируйте WorkbookDesigner с книгой
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            
            // Установите источник данных JSON
            designer.SetJsonDataSource("ds", jsonData);
            
            // Обработать дизайнер
            designer.Process();
            
            // Вывести результат.
            Console.WriteLine("Processed value: " + worksheet.Cells["A2"].StringValue);
        }
    }
}
```

### См. также

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


