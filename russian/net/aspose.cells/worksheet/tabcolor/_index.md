---
title: "Worksheet.TabColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Представляет цвет вкладки листа"
type: docs
url: /ru/net/aspose.cells/worksheet/tabcolor/
---
## Worksheet.TabColor property

Представляет цвет вкладки листа.

```csharp
public Color TabColor { get; set; }
```

### Примечания

Эта функция поддерживается только в ExcelXP (Excel2002) и более поздних версиях. Если сохранить файл в формате Excel97 или Excel2000, она будет опущена.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите цвет вкладки в красный
            worksheet.TabColor = Color.Red;
            Console.WriteLine("Tab color set to: " + worksheet.TabColor);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Очистите цвет вкладки
            worksheet.TabColor = Color.Empty;
            Console.WriteLine("Tab color cleared: " + worksheet.TabColor.IsEmpty);
            
            // Сохранить изменённую книгу
            workbook.Save("output_modified.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


