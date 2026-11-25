---
title: "VbaProjectReferenceCollection.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaProjectReferenceCollection. Copia i riferimenti da un altro progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreferencecollection/copy/
---
## VbaProjectReferenceCollection.Copy method

Copia i riferimenti da un altro progetto VBA.

```csharp
public void Copy(VbaProjectReferenceCollection source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | VbaProjectReferenceCollection | I riferimenti di origine. |

### Esempi

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

### Vedi anche

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


