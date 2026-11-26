---
title: "WorkbookDesigner.LineByLine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookDesigner. Указывает, обрабатывается ли умный маркер построчно"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/linebyline/
---
## WorkbookDesigner.LineByLine property

Указывает, обрабатывается ли умный маркер построчно.

```csharp
[Obsolete("Use range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LineByLine { get; set; }
```

### Примечания

Значение по умолчанию — true. Если False, файл шаблона должен содержать диапазон с именем "_CellsSmartMarkers".

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте диапазонные умные маркеры. Это свойство будет удалено через 12 месяцев, начиная с июля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyLineByLineDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с умными маркерами
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Настроить умные маркеры в листе
            ws.Cells["A1"].PutValue("&RootData.Name");
            ws.Cells["A2"].PutValue("&RootData.Age");
            ws.Cells["A3"].PutValue("&RootData.Department");
            
            // Создать примерные данные
            var employee = new EmployeeData
            {
                Name = "John Doe",
                Age = 35,
                Department = "Sales"
            };
            
            List<EmployeeData> employees = new List<EmployeeData> { employee };

            // Обработать с параметром LineByLine, установленным в false
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = wb,
                LineByLine = false // This is the key property being demonstrated
            };
            
            designer.SetDataSource("RootData", employees);
            designer.Process();

            // Сохранить результат
            wb.Save("output.xlsx");
            
            Console.WriteLine("Workbook processed with LineByLine=false. Output saved to output.xlsx");
        }
    }

    // Простой класс данных для демонстрации
    public class EmployeeData
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public string Department { get; set; }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


