---
title: "Worksheet.AdvancedFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Karmaşık ölçütlerle verileri filtreler"
type: docs
url: /tr/net/aspose.cells/worksheet/advancedfilter/
---
## Worksheet.AdvancedFilter method

Verileri karmaşık ölçütlerle filtreler.

```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo, 
    bool uniqueRecordOnly)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isFilter | Boolean | Listeyi yerinde filtreleyip filtrelemediğini gösterir. |
| listRange | String | Liste aralığı. |
| criteriaRange | String | Kriter aralığı. |
| copyTo | String | Verilerin kopyalanacağı aralık. |
| uniqueRecordOnly | Boolean | Yalnızca benzersiz satırları gösterir veya kopyalar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAdvancedFilterWithBooleanStringStringStringBooleDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Filtreleme için örnek veri oluştur
            // Başlıklar
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            // Kriterler
            worksheet.Cells["A2"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Category");
            worksheet.Cells["C2"].PutValue("Fruits");
            
            // Veri
            worksheet.Cells["A4"].PutValue("Apple");
            worksheet.Cells["B4"].PutValue("Fruits");
            worksheet.Cells["C4"].PutValue(2.5);
            
            worksheet.Cells["A5"].PutValue("Carrot");
            worksheet.Cells["B5"].PutValue("Vegetables");
            worksheet.Cells["C5"].PutValue(1.2);
            
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B6"].PutValue("Fruits");
            worksheet.Cells["C6"].PutValue(1.8);

            // Gelişmiş filtreyi uygula (yerinde filtrele, yalnızca benzersiz kayıtlar)
            worksheet.AdvancedFilter(false, "A4:C6", "A1:C2", null, true);

            // Çalışma kitabını kaydedin
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


