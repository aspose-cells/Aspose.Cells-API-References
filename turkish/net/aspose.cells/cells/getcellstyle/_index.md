---
title: "Cells.GetCellStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen hücrenin stilini al"
type: docs
url: /tr/net/aspose.cells/cells/getcellstyle/
---
## Cells.GetCellStyle method

Verilen hücrenin stilini al.

```csharp
public Style GetCellStyle(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | satır indeksi |
| sütun | Int32 | sütun |

### Dönüş Değeri

belirtilen hücrenin stili.

### Açıklamalar

Dönen stil yalnızca hücre için ayarlanan veya hücrenin satır/kolonundan devralınan stildir; koşullu biçimlendirmeler gibi diğer ayarlar tarafından uygulanan özellikleri içermez.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsMethodGetCellStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // B5 hücresine (satır 4, sütun 1) erişin ve başlangıç stilini ayarlayın
            Cell cell = worksheet.Cells["B5"];
            cell.PutValue("Styled Cell");
            
            // Başlangıç hücre stilini oluşturun ve uygulayın
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.IsBold = true;  // Changed from Bold to IsBold
            initialStyle.BackgroundColor = Color.LightYellow;
            cell.SetStyle(initialStyle);

            try
            {
                // Int32 parametreleriyle (satır 4, sütun 1) GetCellStyle'ı çağırın
                Style cellStyle = worksheet.Cells.GetCellStyle(4, 1);

                // Alınan stil özelliklerini göster
                Console.WriteLine($"Retrieved style - Bold: {cellStyle.Font.IsBold}, Background: {cellStyle.BackgroundColor}");  // Changed from Bold to IsBold

                // Alınan stili değiştir
                cellStyle.Font.IsItalic = true;  // Changed from Italic to IsItalic
                cellStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

                // Değiştirilen stili hücreye geri uygula
                cell.SetStyle(cellStyle);

                Console.WriteLine("GetCellStyle executed successfully. Modified border and font style.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellStyle: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("CellsGetCellStyleWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


