---
title: "VbaModuleCollection.GetDesignerStorage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaModuleCollection-Methode. Stellt die Daten des Designers dar"
type: docs
url: /de/net/aspose.cells.vba/vbamodulecollection/getdesignerstorage/
---
## VbaModuleCollection.GetDesignerStorage method

Stellt die Daten des Designers dar.

```csharp
public byte[] GetDesignerStorage(string name)
```

### Hinweise

Wir unterstützen das Parsen nicht. Nur zum Kopieren.

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit VBA-Projekt
            Workbook workbook = new Workbook();
            
            // Fügen Sie ein Designer-Modul hinzu
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
            
            // Designer-Speicher abrufen (ist zunächst null)
            byte[] storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Initial designer storage: " + (storage == null ? "null" : "exists"));
            
            // Fügen Sie einige Designer-Speicherdaten hinzu
            byte[] sampleData = new byte[] { 0x01, 0x02, 0x03 };
            workbook.VbaProject.Modules.AddDesignerStorage("TestForm", sampleData);
            
            // Designer-Speicher abrufen und anzeigen
            storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Storage after adding: " + (storage == null ? "null" : BitConverter.ToString(storage)));
        }
    }
}
```

### Siehe auch

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


