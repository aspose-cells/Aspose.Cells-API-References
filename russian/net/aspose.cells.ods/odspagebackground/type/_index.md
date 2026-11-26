---
title: "OdsPageBackground.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsPageBackground. Получает и задает тип фона страницы"
type: docs
url: /ru/net/aspose.cells.ods/odspagebackground/type/
---
## OdsPageBackground.Type property

Получает и задает тип фона страницы.

```csharp
public OdsPageBackgroundType Type { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить настройки страницы первого листа
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            
            // Получить фон страницы ODS
            OdsPageBackground background = ps.ODSPageBackground;
            
            // Установить тип фона как графический и настроить его
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicData = File.ReadAllBytes("image1.png");
            background.GraphicType = OdsPageBackgroundGraphicType.Area;
            
            // Сохраните книгу
            workbook.Save("output.ods");
            
            // Перезагрузить сохранённый файл, чтобы проверить настройки
            Workbook verifyWorkbook = new Workbook("output.ods");
            PageSetup verifyPs = verifyWorkbook.Worksheets[0].PageSetup;
            OdsPageBackground verifyBackground = verifyPs.ODSPageBackground;
            
            // Вывести результаты проверки
            Console.WriteLine("Background Type: " + verifyBackground.Type);
            Console.WriteLine("Graphic Type: " + verifyBackground.GraphicType);
        }
    }
}
```

### См. также

* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


