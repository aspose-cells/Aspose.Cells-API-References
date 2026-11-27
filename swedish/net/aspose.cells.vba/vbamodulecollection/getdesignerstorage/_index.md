---
title: "VbaModuleCollection.GetDesignerStorage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaModuleCollection-metoden. Representerar data för Designer"
type: docs
url: /sv/net/aspose.cells.vba/vbamodulecollection/getdesignerstorage/
---
## VbaModuleCollection.GetDesignerStorage method

Representerar data för Designer.

```csharp
public byte[] GetDesignerStorage(string name)
```

### Anmärkningar

Vi stödjer inte att analysera dem. Endast för kopiering.

### Exempel

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
            // Skapa en arbetsbok med VBA-projekt
            Workbook workbook = new Workbook();
            
            // Lägg till en designer-modul
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
            
            // Hämta designer storage (kommer initialt vara null)
            byte[] storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Initial designer storage: " + (storage == null ? "null" : "exists"));
            
            // Lägg till viss designer storage-data
            byte[] sampleData = new byte[] { 0x01, 0x02, 0x03 };
            workbook.VbaProject.Modules.AddDesignerStorage("TestForm", sampleData);
            
            // Hämta och visa designer storage
            storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Storage after adding: " + (storage == null ? "null" : BitConverter.ToString(storage)));
        }
    }
}
```

### Se även

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


