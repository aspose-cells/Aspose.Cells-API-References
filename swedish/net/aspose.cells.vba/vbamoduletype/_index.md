---
title: "Enum VbaModuleType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Vba.VbaModuleType enum. Representerar typen av VBA-modul"
type: docs
url: /sv/net/aspose.cells.vba/vbamoduletype/
---
## VbaModuleType enumeration

Representerar typen av VBA‑modul.

```csharp
public enum VbaModuleType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Procedural | `0` | Representerar en procedurmodul. |
| Document | `1` | Representerar en dokumentmodul. |
| Class | `2` | Representerar en klassmodul. |
| Designer | `3` | Representerar en designermodul. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleTypeDemo
    {
        public static void VbaModuleTypeExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Initiera VBA-projekt
            VbaProject vbaProject = workbook.VbaProject;
            
            // Lägg till en ny klassmodul
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
            
            // Hämta VBA-modulen
            VbaModule vbaModule = vbaProject.Modules[index];
            
            // Ställ in koder för modulen
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
            
            // Spara Excel-filen
            workbook.Save("VbaModuleTypeExample.xlsm");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


