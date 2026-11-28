---
title: "Enum VisibilityType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.VisibilityType enum. Sayfa görünürlüğü durumlarını temsil eder"
type: docs
url: /tr/net/aspose.cells/visibilitytype/
---
## VisibilityType enumeration

Sayfa görünürlüğü durumlarını temsil eder.

```csharp
public enum VisibilityType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Visible | `0` | Sayfanın görünür olduğunu gösterir. |
| Hidden | `1` | Sayfanın gizli olduğunu, ancak kullanıcı arayüzü üzerinden kullanıcı tarafından gösterilebileceğini gösterir. |
| VeryHidden | `2` | Sayfanın gizli olduğunu ve kullanıcı arayüzünde (UI) gösterilemeyeceğini gösterir. Bu durum yalnızca programlama yoluyla kullanılabilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VisibilityTypeDemo
    {
        public static void VisibilityTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("NewSheet");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasının adını ayarlayın
            worksheet.Name = "DemoSheet";

            // Çalışma sayfasının görünürlüğünü Gizli olarak ayarlayın
            worksheet.VisibilityType = VisibilityType.Hidden;

            // Çalışma kitabını kaydedin
            workbook.Save("VisibilityTypeExample.xlsx");

            // İşlemin tamamlandığını göstermek için çıktı
            Console.WriteLine("Workbook saved with the worksheet visibility set to Hidden.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


