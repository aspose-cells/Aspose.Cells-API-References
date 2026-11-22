---
title: "SensitivityLabelCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SensitivityLabelCollection. تضيف تسمية حساسة"
type: docs
url: /ar/net/aspose.cells.metas/sensitivitylabelcollection/add/
---
## SensitivityLabelCollection.Add method

يضيف تصنيف حساسية.

```csharp
public int Add(string id, bool isEnabled, SensitivityLabelAssignmentType methodType, string siteId, 
    SensitivityLabelMarkType markType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| id | String | معرّف التسمية. |
| isEnabled | منطقي | يشير إلى ما إذا كانت هذه التسمية الحساسة مفعّلة. |
| methodType | SensitivityLabelAssignmentType | نوع طريقة التعيين. |
| siteId | String | معرّف الموقع. |
| markType | SensitivityLabelMarkType | نوع العلامة. |

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء SensitivityLabelCollection جديد
            var sensitivityLabels = new SensitivityLabelCollection();
            
            try
            {
                // استدعِ طريقة Add مع معلمات محددة
                int index = sensitivityLabels.Add(
                    id: "Confidential",
                    isEnabled: true,
                    methodType: SensitivityLabelAssignmentType.Privileged,
                    siteId: "Contoso",
                    markType: SensitivityLabelMarkType.Watermark);
                
                Console.WriteLine($"Sensitivity label added at index: {index}");
                
                // أضف بعض البيانات لتوضيح التأثير
                worksheet.Cells["A1"].Value = "Confidential Data";
                worksheet.Cells["A2"].Value = "This document contains sensitive information";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("SensitivityLabelAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabelCollection](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


