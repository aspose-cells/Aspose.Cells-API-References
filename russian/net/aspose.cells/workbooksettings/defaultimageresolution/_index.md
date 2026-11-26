---
title: "WorkbookSettings.DefaultImageResolution"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает и задает разрешение изображения по умолчанию"
type: docs
url: /ru/net/aspose.cells/workbooksettings/defaultimageresolution/
---
## WorkbookSettings.DefaultImageResolution property

Получает и задает разрешение изображения по умолчанию.

```csharp
public int DefaultImageResolution { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultImageResolutionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить разрешение изображения по умолчанию
            workbook.Settings.DefaultImageResolution = 300;
            
            // Добавить лист и вставить изображение
            Worksheet worksheet = workbook.Worksheets[0];
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[imgIndex];
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Проверить разрешение изображения по умолчанию
            Console.WriteLine("Default Image Resolution: " + workbook.Settings.DefaultImageResolution);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


