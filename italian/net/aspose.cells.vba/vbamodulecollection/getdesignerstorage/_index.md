---
title: "VbaModuleCollection.GetDesignerStorage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaModuleCollection. Rappresenta i dati del Designer"
type: docs
url: /it/net/aspose.cells.vba/vbamodulecollection/getdesignerstorage/
---
## VbaModuleCollection.GetDesignerStorage method

Rappresenta i dati del Designer.

```csharp
public byte[] GetDesignerStorage(string name)
```

### Osservazioni

Non supportiamo l'analisi di questi. Solo per la copia.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodGetDesignerStorageWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con progetto VBA
            Workbook workbook = new Workbook();
            
            // Aggiungi un modulo designer
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
            
            // Ottieni l'archiviazione del designer (sarà null inizialmente)
            byte[] storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Initial designer storage: " + (storage == null ? "null" : "exists"));
            
            // Aggiungi alcuni dati di archiviazione del designer
            byte[] sampleData = new byte[] { 0x01, 0x02, 0x03 };
            workbook.VbaProject.Modules.AddDesignerStorage("TestForm", sampleData);
            
            // Ottieni e visualizza l'archiviazione del designer
            storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Storage after adding: " + (storage == null ? "null" : BitConverter.ToString(storage)));
        }
    }
}
```

### Vedi anche

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


