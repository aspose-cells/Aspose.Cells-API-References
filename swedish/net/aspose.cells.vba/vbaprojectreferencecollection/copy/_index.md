---
title: "VbaProjectReferenceCollection.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProjectReferenceCollection metod. Kopierar referenser från ett annat VBA-projekt"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreferencecollection/copy/
---
## VbaProjectReferenceCollection.Copy method

Kopierar referenser från ett annat VBA-projekt.

```csharp
public void Copy(VbaProjectReferenceCollection source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | VbaProjectReferenceCollection | Källreferenserna. |

### Exempel

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

### Se även

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


