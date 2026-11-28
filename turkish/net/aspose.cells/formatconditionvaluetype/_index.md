---
title: "Enum FormatConditionValueType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FormatConditionValueType enum. Koşul değer türü"
type: docs
url: /tr/net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

Koşul değer türü.

```csharp
public enum FormatConditionValueType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Formula | `0` | Gradyan için minimum/ orta / maksimum değer bir formülle belirlenir. |
| Max | `1` | Aralıktaki maksimum değerin gradyan için maksimum değer olarak kullanılacağını gösterir. |
| Min | `2` | Aralıktaki minimum değerin gradyan için minimum değer olarak kullanılacağını gösterir. |
| Number | `3` | Gradyan için minimum / orta / maksimum değerin sabit bir sayısal değerle belirtildiğini gösterir. |
| Percent | `4` | Değer, aralıktaki minimum ve maksimum değerler arasındaki yüzdeyi gösterir ve bu, gradyan için minimum / orta / maksimum değer olarak kullanılır. |
| Percentile | `5` | Değer, aralıktaki yüzde sıralamasını gösterir ve bu, gradyan için minimum / orta / maksimum değer olarak kullanılır. |
| AutomaticMax | `6` | Aralıktaki Otomatik maksimum değerin gradyan için Otomatik maksimum değer olarak kullanılacağını gösterir. |
| AutomaticMin | `7` | Aralıktaki Otomatik minimum değerin gradyan için Otomatik minimum değer olarak kullanılacağını gösterir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFormatConditionValueTypeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Biçim koşulları ekle
            int formatConditionsIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatConditionsIndex];
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[conditionIndex];

            // Simge seti özelliklerini ayarla
            condition.IconSet.Type = IconSetType.Boxes5;
            condition.IconSet.ShowValue = false;
            condition.IconSet.Reverse = true;

            // Hücre değerini ayarla ve biçimlendirmeyi uygula
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Boxes5 Icon Set Example");

            // Biçim koşulu değer türüne eriş
            FormatConditionValueType valueType = condition.IconSet.Cfvos[0].Type;
            Console.WriteLine("First CFVO Type: " + valueType);

            // Simge seti koşullarından değerleri göster
            Console.WriteLine("\nIcon Set Threshold Values:");
            foreach (ConditionalFormattingValue cfvo in condition.IconSet.Cfvos)
            {
                Console.WriteLine($"Type: {cfvo.Type}, Value: {cfvo.Value}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("FormatConditionValueTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


