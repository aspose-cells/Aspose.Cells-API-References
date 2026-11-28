---
title: "ListColumn.SetCustomCalculatedFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListColumn yöntemi. Bu liste sütunu için formülü ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/listcolumn/setcustomcalculatedformula/
---
## ListColumn.SetCustomCalculatedFormula method

Bu liste sütunu için formülü ayarlar.

```csharp
public void SetCustomCalculatedFormula(string formula, bool isR1C1, bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | bu liste sütunu için formül. |
| isR1C1 | Boolean | Formülün R1C1 olarak biçimlendirilmesi gerekip gerekmediği. |
| isLocal | Boolean | Formülün yerel ayarlara göre biçimlendirilmesi gerekip gerekmediği. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnMethodSetCustomCalculatedFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tablo için örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Total");

            // Tablo oluşturun
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true); // Adjusted parameters to match correct overload
            ListObject table = worksheet.ListObjects[tableIndex];

            // İkinci liste sütununu al
            ListColumn totalColumn = table.ListColumns[1];

            try
            {
                // Standart yerel ayar ile A1 notasyonu kullanarak özel formül ayarla
                totalColumn.SetCustomCalculatedFormula("=A2*1.1", false, false);
                
                Console.WriteLine("Custom formula set successfully.");
                Console.WriteLine($"Cell B2 formula: {worksheet.Cells["B2"].Formula}");
                Console.WriteLine($"Cell B3 formula: {worksheet.Cells["B3"].Formula}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("SetCustomCalculatedFormulaExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


