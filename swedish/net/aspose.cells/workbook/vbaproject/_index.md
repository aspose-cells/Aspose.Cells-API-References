---
title: "Workbook.VbaProject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar VbaProject i ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/workbook/vbaproject/
---
## Workbook.VbaProject property

Hämtar `VbaProject` i ett kalkylblad.

```csharp
public VbaProject VbaProject { get; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyVbaProjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till VBA-projektet (VbaProject är skrivskyddat, vi kan bara kontrollera om det finns)
            if (workbook.VbaProject == null)
            {
                // Skapa VBA-projekt genom att spara som makroaktiverad arbetsbok
                workbook.Save("temp.xlsm", SaveFormat.Xlsm);
                workbook = new Workbook("temp.xlsm");
                File.Delete("temp.xlsm");
            }

            // Lägg till en ny modul i VBA-projektet
            int moduleIndex = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Hämta den tillagda modulen och ange dess kod
            VbaModule module = workbook.VbaProject.Modules[moduleIndex];
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";

            // Spara arbetsboken
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "VbaProjectDemo.xlsm");
            workbook.Save(outputPath, SaveFormat.Xlsm);
        }
    }
}
```

### Se även

* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


