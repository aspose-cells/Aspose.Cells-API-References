---
title: "SensitivityLabelCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SensitivityLabelCollection yöntemi. Bir hassasiyet etiketi ekler"
type: docs
url: /tr/net/aspose.cells.metas/sensitivitylabelcollection/add/
---
## SensitivityLabelCollection.Add method

Bir hassasiyet etiketi ekler.

```csharp
public int Add(string id, bool isEnabled, SensitivityLabelAssignmentType methodType, string siteId, 
    SensitivityLabelMarkType markType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| id | String | Etiketin kimliği. |
| isEnabled | Boolean | Bu hassasiyet etiketinin etkin olup olmadığını gösterir. |
| methodType | SensitivityLabelAssignmentType | Atama yöntemi türü. |
| siteId | String | Sitenin kimliği. |
| markType | SensitivityLabelMarkType | İşaret türü. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelCollectionMethodAddWithStringBooleanSensitivityLabelADemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yeni bir SensitivityLabelCollection oluşturun
            var sensitivityLabels = new SensitivityLabelCollection();
            
            try
            {
                // Add metodunu belirli parametrelerle çağırın
                int index = sensitivityLabels.Add(
                    id: "Confidential",
                    isEnabled: true,
                    methodType: SensitivityLabelAssignmentType.Privileged,
                    siteId: "Contoso",
                    markType: SensitivityLabelMarkType.Watermark);
                
                Console.WriteLine($"Sensitivity label added at index: {index}");
                
                // Etkiyi göstermek için bazı verileri ekleyin
                worksheet.Cells["A1"].Value = "Confidential Data";
                worksheet.Cells["A2"].Value = "This document contains sensitive information";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("SensitivityLabelAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabelCollection](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


