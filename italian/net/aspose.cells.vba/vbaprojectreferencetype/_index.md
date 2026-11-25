---
title: "Enum VbaProjectReferenceType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Vba.VbaProjectReferenceType. Rappresenta il tipo di riferimento al progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreferencetype/
---
## VbaProjectReferenceType enumeration

Rappresenta il tipo di riferimento del progetto VBA.

```csharp
public enum VbaProjectReferenceType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Registered | `0` | Specifica un riferimento a una libreria di tipi Automation. |
| Control | `1` | Specifica un riferimento a una libreria di tipi modificata e alla sua libreria di tipi estesa. |
| Project | `2` | Specifica un riferimento a un progetto VBA esterno. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferenceTypeDemo
    {
        public static void VbaProjectReferenceTypeExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Inizializza progetto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Aggiungi riferimento al progetto VBA
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Salvataggio del file Excel
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");

            // Dimostrazione dell'uso dell'enum VbaProjectReferenceType
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


