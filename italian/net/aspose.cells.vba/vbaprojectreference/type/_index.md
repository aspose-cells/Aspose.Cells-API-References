---
title: "VbaProjectReference.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "VbaProjectReference proprietà. Ottiene il tipo di questo riferimento"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreference/type/
---
## VbaProjectReference.Type property

Ottiene il tipo di questo riferimento.

```csharp
public VbaProjectReferenceType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Inizializza il progetto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Aggiungi un riferimento registrato al progetto VBA
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Ottieni il primo riferimento e dimostra la proprietà Type
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);

            // Salva la cartella di lavoro
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");
        }
    }
}
```

### Vedi anche

* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


