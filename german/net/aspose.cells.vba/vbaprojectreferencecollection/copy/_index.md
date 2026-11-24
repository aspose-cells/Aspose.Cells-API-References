---
title: "VbaProjectReferenceCollection.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProjectReferenceCollection-Methode. Kopiert Referenzen aus einem anderen VBA-Projekt"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreferencecollection/copy/
---
## VbaProjectReferenceCollection.Copy method

Kopiert Verweise aus einem anderen VBA-Projekt.

```csharp
public void Copy(VbaProjectReferenceCollection source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | VbaProjectReferenceCollection | Die Quellreferenzen. |

### Beispiele

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

### Siehe auch

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


