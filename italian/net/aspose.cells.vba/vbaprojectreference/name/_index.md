---
title: "VbaProjectReference.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "VbaProjectReference proprietà. Ottiene e imposta il nome del riferimento"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreference/name/
---
## VbaProjectReference.Name property

Ottiene e imposta il nome del riferimento.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyNameDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro (il progetto VBA viene creato automaticamente per i file .xlsm)
            Workbook workbook = new Workbook(FileFormatType.Xlsm);
            
            // Aggiungi un riferimento al progetto VBA
            string referenceName = "MyReference";
            string referencePath = @"C:\Temp\MyLibrary.dll";
            workbook.VbaProject.References.AddRegisteredReference(referenceName, referencePath);

            // Accedi e verifica il riferimento tramite la proprietà Name
            VbaProjectReferenceCollection references = workbook.VbaProject.References;
            for (int i = 0; i < references.Count; i++)
            {
                if (references[i].Name.Equals(referenceName))
                {
                    Console.WriteLine($"Found reference: {references[i].Name}");
                    break;
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("VbaProjectReferenceDemo.xlsm");
        }
    }
}
```

### Vedi anche

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


