---
title: "FindOptions.Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions özelliği. Aranacak format"
type: docs
url: /tr/net/aspose.cells/findoptions/style/
---
## FindOptions.Style property

Aranacak format.

```csharp
public Style Style { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Mavi yazı tipiyle bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Blue;

            // Stili F2 hücresine uygula
            Cell cell = worksheet.Cells["F2"];
            cell.PutValue("SearchTarget");
            cell.SetStyle(style);

            // Stili kullanarak find options oluştur
            FindOptions options = new FindOptions();
            options.Style = style;

            // Eşleşen stile sahip hücreyi bul
            Cell foundCell = worksheet.Cells.Find(null, null, options);

            // Bulunan hücrenin adını çıktı olarak ver
            Console.WriteLine("Cell found with matching style: " + foundCell?.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


