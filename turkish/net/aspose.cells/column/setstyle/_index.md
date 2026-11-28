---
title: "Column.SetStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Column yöntemi. Bu sütunun stilini ayarlar"
type: docs
url: /tr/net/aspose.cells/column/setstyle/
---
## Column.SetStyle method

Bu sütunun stilini ayarlar.

```csharp
public void SetStyle(Style style)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Bu sütundaki hücreler için varsayılan stil olarak kullanılacak stil. |

### Açıklamalar

Bu yöntem, verilen stili bu sütun için varsayılan stil olarak ayarlar, aynı sütundaki mevcut hücrelerin stil ayarlarını değiştirmez. Mevcut hücrelerin stil ayarlarını aynı anda belirtilen stile güncellemek için lütfen [`ApplyStyle`](../applystyle/) kullanın.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnMethodSetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk sütuna eriş
            Column column = worksheet.Cells.Columns[0];

            // Çalışma kitabından yeni bir stil oluştur
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            try
            {
                // Özel stili tüm sütuna uygula
                column.SetStyle(style);
                
                Console.WriteLine($"Style applied successfully to column {column.Index}");
                Console.WriteLine($"Font: {style.Font.Name}, Size: {style.Font.Size}, Bold: {style.Font.IsBold}");
                Console.WriteLine($"Background: {style.ForegroundColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("ColumnMethodSetStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


