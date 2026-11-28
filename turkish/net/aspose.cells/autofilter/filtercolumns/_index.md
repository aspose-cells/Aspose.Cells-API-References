---
title: "AutoFilter.FilterColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter özelliği. Filtre sütunlarının koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/autofilter/filtercolumns/
---
## AutoFilter.FilterColumns property

Filtre sütunlarının koleksiyonunu alır.

```csharp
public FilterColumnCollection FilterColumns { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyFilterColumnsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Status");
            
            worksheet.Cells["A2"].PutValue("HR");
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["C2"].PutValue("Present");
            
            worksheet.Cells["A3"].PutValue("IT");
            worksheet.Cells["B3"].PutValue("Sarah");
            worksheet.Cells["C3"].PutValue("Absent");
            
            worksheet.Cells["A4"].PutValue("HR");
            worksheet.Cells["B4"].PutValue("Mike");
            worksheet.Cells["C4"].PutValue("Present");

            // Otomatik filtre uygula
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:C1";
            
            // "Present" değerleri için 2. sütunu (Status) filtrele
            autoFilter.Filter(2, "Present");
            
            // Filtre sütununa eriş
            FilterColumn filterColumn = autoFilter.FilterColumns[2];
            
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


