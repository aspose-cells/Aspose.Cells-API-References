---
title: "Range.ClearHyperlinks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Yalnızca hiperlinkleri kaldırır"
type: docs
url: /tr/net/aspose.cells/range/clearhyperlinks/
---
## Range.ClearHyperlinks method

Yalnızca köprüleri kaldırır.

```csharp
public void ClearHyperlinks(bool clearFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| clearFormat | Boolean | Hiperlinklerin biçimini temizleyip temizlemeyeceğini gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearHyperlinksWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralık oluştur ve gösterim için bazı hiperlinkler ekle
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");
            range.AddHyperlink("https://www.example.com", "Example", "Visit Example");

            try
            {
                // Biçim koruması ile bağlantıları temizle (false)
                range.ClearHyperlinks(false);
                Console.WriteLine("Hyperlinks cleared while preserving format");

                // Bağlantıları tekrar ekle
                range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");

                // Biçim koruması olmadan bağlantıları temizle (true)
                range.ClearHyperlinks(true);
                Console.WriteLine("Hyperlinks cleared without preserving format");

                // Çalışma kitabını kaydedin
                workbook.Save("ClearHyperlinksDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


