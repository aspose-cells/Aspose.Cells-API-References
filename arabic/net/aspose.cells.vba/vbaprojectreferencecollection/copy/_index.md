---
title: "VbaProjectReferenceCollection.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaProjectReferenceCollection. ينسخ الإشارات من مشروع VBA آخر"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreferencecollection/copy/
---
## VbaProjectReferenceCollection.Copy method

ينسخ المراجع من مشروع VBA آخر.

```csharp
public void Copy(VbaProjectReferenceCollection source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | VbaProjectReferenceCollection | المراجع المصدرية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferenceCollectionMethodCopyWithVbaProjectReferenceCollectionDemo
    {
        public static void Run()
        {
            Workbook sourceWorkbook = new Workbook();
            sourceWorkbook.VbaProject.References.AddRegisteredReference(
                "stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation"
            );

            Workbook targetWorkbook = new Workbook();

            try
            {
                targetWorkbook.VbaProject.References.Copy(sourceWorkbook.VbaProject.References);
                Console.WriteLine($"Copied {sourceWorkbook.VbaProject.References.Count} VBA references to target workbook");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error copying references: {ex.Message}");
            }

            targetWorkbook.Save("VbaReferenceCopyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


