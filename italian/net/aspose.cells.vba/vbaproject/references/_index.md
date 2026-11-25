---
title: "VbaProject.References"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaProject. Ottiene tutti i riferimenti del progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/references/
---
## VbaProject.References property

Ottiene tutti i riferimenti del progetto VBA.

```csharp
public VbaProjectReferenceCollection References { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyReferencesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro (il progetto VBA viene creato automaticamente per i file .xlsm)
            Workbook workbook = new Workbook();
            
            // Accedi ai riferimenti del progetto VBA (disponibile solo se la cartella di lavoro ha un progetto VBA)
            if (workbook.VbaProject != null)
            {
                VbaProjectReferenceCollection references = workbook.VbaProject.References;
                
                // Aggiungi diversi tipi di riferimenti
                references.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
                references.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "", "");
                references.AddProjectRefrernce("MyProject", "C:\\Projects\\MyProject.xlam", "..\\MyProject.xlam");

                // Visualizza il conteggio dei riferimenti
                Console.WriteLine($"Total references: {references.Count}");
            }

            // Salva come cartella di lavoro con macro abilitata
            workbook.Save("VbaProjectWithReferences.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Vedi anche

* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


