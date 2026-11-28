---
title: "Enum LookInType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LookInType enum. Arama türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/lookintype/
---
## LookInType enumeration

İçine bakma türünü temsil eder.

```csharp
public enum LookInType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Formulas | `0` | Hücre bir formül ise formülden ([`Formula`](../cell/formula/)) aranan nesneyi bulur, aksi takdirde hücrenin orijinal değerinden (OriginalValues ile aynı) bulur. |
| Values | `1` | Hücrenin orijinal değerinden ([`Value`](../cell/value/)) ve biçimlendirilmiş değerinden ([`StringValue`](../cell/stringvalue/)) nesneyi bulur. |
| ValuesExcludeFormulaCell | `2` | Formül olan hücreleri yok sayar. Formül olmayan hücreler için, Values ile aynı davranır. |
| Comments | `3` | Yalnızca hücrenin yorumundan nesneyi bulur. Yorum olmayan hücreleri yok sayar. |
| OnlyFormulas | `4` | Formül olmayan hücreleri yok sayar. Formül olan hücreler için, formülden ([`Formula`](../cell/formula/)) aranan nesneyi bulur. |
| OriginalValues | `5` | Yalnızca hücrenin orijinal değerinden nesneyi bulur. |
| FormattedValues | `6` | Yalnızca hücrenin biçimlendirilmiş değerinden ([`StringValue`](../cell/stringvalue/)) nesneyi bulur. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassLookInTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı veri ve formüller ekle
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].Formula = "=A1";
            worksheet.Cells["C1"].PutValue("Contains B1");

            // "B1" içeren formül bulunan hücreyi bul
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            Cell foundCell = worksheet.Cells.Find("B1", null, options);

            // Sonucu çıktı olarak ver
            if (foundCell != null)
            {
                Console.WriteLine($"Found cell at row: {foundCell.Row}, column: {foundCell.Column}");
                Console.WriteLine($"Cell value: {foundCell.StringValue}");
                Console.WriteLine($"Cell formula: {foundCell.Formula}");
            }
            else
            {
                Console.WriteLine("Cell not found");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


