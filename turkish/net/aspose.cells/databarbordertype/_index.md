---
title: "Enum DataBarBorderType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataBarBorderType enum. Veri çubuğunun kenar türünü belirtir"
type: docs
url: /tr/net/aspose.cells/databarbordertype/
---
## DataBarBorderType enumeration

Bir veri çubuğunun kenarlık türünü belirtir.

```csharp
public enum DataBarBorderType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Veri çubuğunun kenarı yok. |
| Solid | `1` | Veri çubuğunun katı kenarı vardır. |

### Örnekler

```csharp
using Aspose.Cells;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderTypeDemo
    {
        public static void DataBarBorderTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Çalışma sayfasına koşullu biçimlendirme ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme için bir hücre alanı tanımla
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // Veri çubuğu koşullu biçimlendirme kuralı ekle
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            // DataBar nesnesine eriş
            DataBar dataBar = fc.DataBar;

            // Veri çubuğunun rengini ayarla
            dataBar.Color = Color.Blue;

            // Veri çubuğunun minimum ve maksimum uzunluğunu ayarla
            dataBar.MinLength = 10;
            dataBar.MaxLength = 90;

            // Veri çubuğunun kenarlık tipini ayarla
            dataBar.BarBorder.Type = DataBarBorderType.Solid;

            // Veri çubuğunun kenarlık rengini ayarla
            dataBar.BarBorder.Color = Color.Red;

            // Çalışma kitabını kaydedin
            workbook.Save("DataBarBorderTypeExample.xlsx");
            workbook.Save("DataBarBorderTypeExample.pdf");

            Console.WriteLine("DataBarBorderTypeExample executed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


