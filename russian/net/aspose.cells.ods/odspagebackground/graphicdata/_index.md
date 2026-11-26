---
title: "OdsPageBackground.GraphicData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsPageBackground. Получает и задает графические данные"
type: docs
url: /ru/net/aspose.cells.ods/odspagebackground/graphicdata/
---
## OdsPageBackground.GraphicData property

Получает и задает графические данные.

```csharp
public byte[] GraphicData { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyGraphicDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и его настройкам страницы
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Установите свойства фона страницы ODS
            OdsPageBackground background = pageSetup.ODSPageBackground;
            background.Type = OdsPageBackgroundType.Graphic;
            
            // Загрузите данные изображения и установите их в качестве фона
            string imagePath = "sample.png"; // Replace with actual image path
            if (File.Exists(imagePath))
            {
                background.GraphicData = File.ReadAllBytes(imagePath);
                background.GraphicType = OdsPageBackgroundGraphicType.Area;
                
                // Сохраните книгу
                workbook.Save("output.ods");
                
                Console.WriteLine("ODS file with graphic background created successfully.");
            }
            else
            {
                Console.WriteLine("Image file not found: " + imagePath);
            }
        }
    }
}
```

### См. также

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


