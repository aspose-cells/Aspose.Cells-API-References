---
title: "Workbook.CountOfStylesInPool"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Stil havuzundaki stillerin sayısını alır"
type: docs
url: /tr/net/aspose.cells/workbook/countofstylesinpool/
---
## Workbook.CountOfStylesInPool property

Stil havuzundaki stil sayısını alır.

```csharp
public int CountOfStylesInPool { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCountOfStylesInPoolDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Havuzdaki stil sayısının başlangıç değerini al
            int initialStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Initial styles in pool: {initialStyleCount}");

            // Hücreleri değiştirerek bazı stiller ekle
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Stil 1
            Style style1 = wb.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            cells["A1"].SetStyle(style1);
            
            // Stil 2
            Style style2 = wb.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            style2.Pattern = BackgroundType.Solid;
            cells["B1"].SetStyle(style2);

            // Güncellenmiş stil sayısını al
            int updatedStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Styles after modifications: {updatedStyleCount}");

            // Stil kalıcılığını göstermek için kaydet
            wb.Save("output.html", SaveFormat.Html);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


