---
title: "WorksheetCollection.CreateUnionRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Aralığın adresinden bir Range nesnesi oluşturur"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/createunionrange/
---
## WorksheetCollection.CreateUnionRange method

Bir [`Range`](../../range/) nesnesini aralığın adresinden oluşturur.

```csharp
public UnionRange CreateUnionRange(string address, int sheetIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| address | String | Aralığın adresi. |
| sheetIndex | Int32 | Sayfa indeksi. |

### Dönüş Değeri

Bir [`Range`](../../range/) nesnesi

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateUnionRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Adres dizgelerinden bir birleşik aralık oluştur
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Tüm birleşim aralığı için değeri ayarla.
            unionRange.Value = "Test";
            
            // Birleşik aralığa stil uygula
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Font.IsBold = true;
            unionRange.ApplyStyle(style, new StyleFlag { FontBold = true, FontColor = true });
            
            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../../unionrange/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


