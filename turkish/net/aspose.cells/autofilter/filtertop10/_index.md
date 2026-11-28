---
title: "AutoFilter.FilterTop10"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Listedeki ilk 10 öğeyi filtrele"
type: docs
url: /tr/net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Listede ilk 10 öğeyi filtrele

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | Int32 | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan field 0'dır). |
| isTop | Boolean | Filtrenin üstten mi yoksa alttan mı uygulanacağını gösterir |
| isPercent | Boolean | Öğelerin yüzde mi yoksa sayı mı olduğunu gösterir |
| itemCount | Int32 | Öğe sayısı |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterTop10WithInt32BooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekle (5 satır x 3 sütun sayısal değerlerle)
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Numbers");
            cells["A2"].PutValue(50);
            cells["A3"].PutValue(30);
            cells["A4"].PutValue(80);
            cells["A5"].PutValue(20);
            cells["A6"].PutValue(90);

            // Otomatik filtre aralığını ayarla
            worksheet.AutoFilter.Range = "A1:A6";

            // İlk 10 filtreyi uygula (ilk 2 öğeyi göstererek)
            worksheet.AutoFilter.FilterTop10(0, true, false, 2);

            // Filtreyi yenile
            worksheet.AutoFilter.Refresh();

            // Çalışma kitabını kaydedin
            workbook.Save("FilterTop10Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


