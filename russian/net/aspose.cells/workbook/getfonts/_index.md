---
title: "Workbook.GetFonts"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Получает все шрифты из пула стилей"
type: docs
url: /ru/net/aspose.cells/workbook/getfonts/
---
## Workbook.GetFonts method

Получает все шрифты в пуле стилей.

```csharp
public Font[] GetFonts()
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetFontsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте ячейки с разными шрифтами
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["A2"].PutValue("Sample Text 2");
            
            // Получайте и изменяйте шрифты
            Font font1 = worksheet.Cells["A1"].GetStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            
            Font font2 = worksheet.Cells["A2"].GetStyle().Font;
            font2.Name = "Times New Roman";
            font2.Size = 14;
            font2.IsBold = true;

            // Получить все шрифты, используемые в рабочей книге
            Font[] fonts = workbook.GetFonts();
            Console.WriteLine("Total fonts in workbook: " + fonts.Length);
            
            // Отобразить информацию о шрифте
            foreach (Font font in fonts)
            {
                Console.WriteLine($"Font: {font.Name}, Size: {font.Size}, Bold: {font.IsBold}");
            }
            
            // Сохраните и перезагрузите, чтобы продемонстрировать сохранность
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Workbook loadedWorkbook = new Workbook(stream);
                Console.WriteLine("Fonts after save/load: " + loadedWorkbook.GetFonts().Length);
            }
        }
    }
}
```

### См. также

* class [Font](../../font/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


