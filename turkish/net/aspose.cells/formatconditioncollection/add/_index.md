---
title: "FormatConditionCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatConditionCollection yöntemi. Bir biçimlendirme koşulu ve etkilenen hücre aralığını FormatConditions'a ekler. FormatConditions en fazla üç koşullu biçimlendirme içerebilir. Koşullu biçimlendirme formüllerinde diğer sayfalara referans verilmesine izin verilmez."
type: docs
url: /tr/net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

Bir biçimlendirme koşulu ve etkilenen hücre aralığını FormatConditions'a ekler. FormatConditions en fazla üç koşullu biçim içerebilir. Koşullu biçimlendirme formüllerinde diğer sayfalara referans verilmesine izin verilmez.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | CellArea | Koşullu biçimlendirilmiş hücre aralığı. |
| type | FormatConditionType | Koşullu biçimlendirme türü. FormatConditionType üyesi olabilir. |
| operatorType | OperatorType | Karşılaştırma operatörü. OperatorType üyesi olabilir. |
| formula1 | String | Koşullu biçimlendirme ile ilişkili değer veya ifade. |
| formula2 | String | Koşullu biçimlendirme ile ilişkili değer veya ifade |

### Dönüş Değeri

[0]:Formatting condition object index;[1] Effected cell rang index.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddWithCellAreaFormatConditionTypeOpeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Örnek verileri doldur
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Koşullu biçimlendirme ekle
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            
            // Belirtilen parametrelerle Add metodunu göster
            fcc.Add(
                CellArea.CreateCellArea(0, 0, 4, 0),
                FormatConditionType.Expression,
                OperatorType.None,
                "=A1>AVERAGE(OFFSET($A$1:$A$5,0,0)-0)",
                null
            );

            // Biçimlendirmeyi uygula
            int fontSize = wb.DefaultStyle.Font.Size;
            fcc[0].Style.Font.Size = fontSize + 2;

            // Sonucu göstermek için çalışma kitabını kaydet
            wb.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


