---
title: "WorksheetCollection.SensitivityLabels"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. Tüm hassasiyet etiketlerini temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/sensitivitylabels/
---
## WorksheetCollection.SensitivityLabels property

Tüm hassasiyet etiketlerini temsil eder.

```csharp
public SensitivityLabelCollection SensitivityLabels { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metas;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertySensitivityLabelsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfası koleksiyonuna eriş.
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Bir hassasiyet etiketi ekle
            int index = worksheets.SensitivityLabels.Add(
                "{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", // ID
                true,                                       // IsEnabled
                SensitivityLabelAssignmentType.Standard,     // AssignmentType
                "contoso-site",                             // SiteId
                SensitivityLabelMarkType.Header              // MarkType
            );
            
            // Eklenen etiketi doğrula
            SensitivityLabel label = worksheets.SensitivityLabels[index];
            Console.WriteLine($"Label added - ID: {label.Id}, SiteID: {label.SiteId}");
            
            // Çalışma kitabını kaydedin
            workbook.Save("SensitivityLabelsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SensitivityLabelCollection](../../../aspose.cells.metas/sensitivitylabelcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


