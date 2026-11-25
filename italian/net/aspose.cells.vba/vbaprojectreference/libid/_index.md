---
title: "VbaProjectReference.Libid"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaProjectReference. Ottiene e imposta il Libid del riferimento"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreference/libid/
---
## VbaProjectReference.Libid property

Ottiene e imposta il Libid del riferimento.

```csharp
public string Libid { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyLibidDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook targetWorkbook = new Workbook();
            
            // Carica la cartella di lavoro di origine con il progetto VBA
            Workbook sourceWorkbook = new Workbook("source.xlsm");
            
            // Cancella i riferimenti esistenti nel target
            targetWorkbook.VbaProject.References.Clear();
            
            // Copia i riferimenti dalla sorgente alla destinazione
            foreach (VbaProjectReference reference in sourceWorkbook.VbaProject.References)
            {
                if (reference.Type == VbaProjectReferenceType.Registered)
                {
                    // Dimostra l'uso della proprietà Libid
                    targetWorkbook.VbaProject.References.AddRegisteredReference(reference.Name, reference.Libid);
                }
                else if (reference.Type == VbaProjectReferenceType.Control)
                {
                    targetWorkbook.VbaProject.References.AddControlRefrernce(
                        reference.Name, 
                        reference.Libid, 
                        reference.Twiddledlibid, 
                        reference.ExtendedLibid);
                }
            }
            
            // Salva il risultato
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### Vedi anche

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


