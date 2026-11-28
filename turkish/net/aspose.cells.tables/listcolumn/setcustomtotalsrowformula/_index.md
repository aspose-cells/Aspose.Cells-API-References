---
title: "ListColumn.SetCustomTotalsRowFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListColumn metodu. Bu liste sütununun toplam satırının formülünü alır"
type: docs
url: /tr/net/aspose.cells.tables/listcolumn/setcustomtotalsrowformula/
---
## ListColumn.SetCustomTotalsRowFormula method

Bu liste sütununun toplam satırının formülünü alır.

```csharp
public void SetCustomTotalsRowFormula(string formula, bool isR1C1, bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | bu liste sütunu için formül. |
| isR1C1 | Boolean | Formülün R1C1 olarak biçimlendirilmesi gerekip gerekmediği. |
| isLocal | Boolean | Formülün yerel ayarlara göre biçimlendirilmesi gerekip gerekmediği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetCustomTotalsRowFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // Bir liste nesnesi oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Toplam satırını etkinleştir ve özel formül ayarla
            listObject.ShowTotals = true;
            listObject.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
            listObject.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


