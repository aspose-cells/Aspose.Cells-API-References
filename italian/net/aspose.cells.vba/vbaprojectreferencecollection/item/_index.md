---
title: "VbaProjectReferenceCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaProjectReferenceCollection. Ottieni il riferimento nell'elenco per indice"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreferencecollection/item/
---
## VbaProjectReferenceCollection indexer

Ottieni il riferimento nella lista per indice.

```csharp
public VbaProjectReference this[int i] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| i | L'indice. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Inizializza il progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Aggiungi riferimenti al progetto VBA
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            vbaProject.References.AddControlRefrernce("MSForms", 
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", 
                "twiddledLibid", "extendedLibid");
            
            // Ottieni la raccolta dei riferimenti
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Accedi ai riferimenti usando la proprietà Item
            VbaProjectReference firstRef = references[0];
            VbaProjectReference secondRef = references[1];
            
            Console.WriteLine("First Reference: " + firstRef.Name);
            Console.WriteLine("Second Reference: " + secondRef.Name);
            
            // Salva la cartella di lavoro
            workbook.Save("VbaProjectReferences.xlsm");
        }
    }
}
```

### Vedi anche

* class [VbaProjectReference](../../vbaprojectreference/)
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


