---
title: "WorkbookSettings.UpdateAdjacentCellsBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Bitişik hücrelerin kenarlığının güncellenip güncellenmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/updateadjacentcellsborder/
---
## WorkbookSettings.UpdateAdjacentCellsBorder property

Komşu hücrelerin kenarlığını güncelleyip güncellemeyeceğini belirtir.

```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur. Örneğin: A1 hücresinin alt kenarı güncellenirse, A2 hücresinin üst kenarı da değiştirilmelidir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateAdjacentCellsBorderDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Komşu hücrelerin kenarlıklarını güncellemeyi etkinleştir
            workbook.Settings.UpdateAdjacentCellsBorder = true;

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine değer ayarla ve kenarlık uygula
            worksheet.Cells["A1"].PutValue("Sample");
            Style styleA1 = workbook.CreateStyle();
            styleA1.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            styleA1.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(styleA1);

            // Komşu hücre B1'e (A1'in sağında) değer ayarla
            worksheet.Cells["B1"].PutValue("Adjacent");

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            Console.WriteLine("Workbook saved with adjacent cell border update enabled.");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


