---
title: "Cell.GetPrecedents"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bu hücrenin formülünde görünen tüm referansları alır"
type: docs
url: /tr/net/aspose.cells/cell/getprecedents/
---
## Cell.GetPrecedents method

Bu hücrenin formülünde görünen tüm referansları al.

```csharp
public ReferredAreaCollection GetPrecedents()
```

### Dönüş Değeri

Bu hücrenin formülünde görünen tüm referansların koleksiyonu.

### Açıklamalar

Bu bir formül hücresi değilse null döndürür. Bu hücrenin formülünde görünen tüm referanslar, hesaplama sırasında referans alınsalar da alınmasalar da döndürülür. Örneğin, "=IF(TRUE,A1,A2)" formülündeki A2 hücresi hesaplama sırasında kullanılmasa da hâlâ formülün öncülleri olarak kabul edilir. Yalnızca hesaplamayı etkileyen referansları elde etmek için lütfen [`GetPrecedentsInCalculation`](../getprecedentsincalculation/) kullanın.

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Öncüllerle formül ayarla
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1";
            
            // Tüm öncül referansları al
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Her öncül referansı göster
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                Console.WriteLine(sb.ToString());
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ReferredAreaCollection](../../referredareacollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


