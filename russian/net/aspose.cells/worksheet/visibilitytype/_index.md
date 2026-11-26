---
title: "Worksheet.VisibilityType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает видимое состояние этого листа"
type: docs
url: /ru/net/aspose.cells/worksheet/visibilitytype/
---
## Worksheet.VisibilityType property

Указывает видимое состояние этого листа.

```csharp
public VisibilityType VisibilityType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVisibilityTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить листы
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Установить разные типы видимости для каждого листа
            workbook.Worksheets[0].VisibilityType = VisibilityType.Hidden;
            workbook.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
            workbook.Worksheets[2].VisibilityType = VisibilityType.Visible;

            // Сохраните книгу
            string outputPath = "output_visibility.xlsx";
            workbook.Save(outputPath);

            // Перезагрузить книгу, чтобы проверить настройки видимости
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Вывести типы видимости
            Console.WriteLine("Worksheet 0 Visibility: " + loadedWorkbook.Worksheets[0].VisibilityType);
            Console.WriteLine("Worksheet 1 Visibility: " + loadedWorkbook.Worksheets[1].VisibilityType);
            Console.WriteLine("Worksheet 2 Visibility: " + loadedWorkbook.Worksheets[2].VisibilityType);
        }
    }
}
```

### См. также

* enum [VisibilityType](../../visibilitytype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


