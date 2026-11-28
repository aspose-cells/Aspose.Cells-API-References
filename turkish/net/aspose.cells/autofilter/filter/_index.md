---
title: "AutoFilter.Filter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Belirtilen kriterlere göre bir listeyi filtreler"
type: docs
url: /tr/net/aspose.cells/autofilter/filter/
---
## AutoFilter.Filter method

Listeyi belirtilen ölçütlerle filtreler.

```csharp
public void Filter(int fieldIndex, string criteria)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | Int32 | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan field 0'dır). |
| kriter | String | Belirtilen kriter (bir dize; örneğin, "101"). |

### Açıklamalar

Aspose.Cells, bu alandaki diğer tüm filtre ayarlarını MS Excel 97-2003 gibi kaldıracaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("Nom1");
            sheet.Cells["A3"].PutValue("Nom2");
            sheet.Cells["A4"].PutValue("Nom3");
            sheet.Cells["A5"].PutValue("Nom2");

            // Doğru SetRange parametrelerini kullanarak otomatik filtreyi uygulayın
            sheet.AutoFilter.SetRange(0, 0, 4); // startRow: 0, startColumn: 0, endRow: 4
            sheet.AutoFilter.Filter(0, "Nom2"); // Filter column 0 (A) for "Nom2"
            sheet.AutoFilter.Refresh();

            // Sonucu kaydet
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


