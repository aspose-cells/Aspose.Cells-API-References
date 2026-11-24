---
title: "Workbook.VbaProject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt das VbaProject in einer Tabelle zurück"
type: docs
url: /de/net/aspose.cells/workbook/vbaproject/
---
## Workbook.VbaProject property

Gibt das `VbaProject` in einer Tabelle zurück.

```csharp
public VbaProject VbaProject { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das VBA‑Projekt zu (VbaProject ist schreibgeschützt, wir können nur prüfen, ob es existiert)
            if (workbook.VbaProject == null)
            {
                // Erstelle ein VBA‑Projekt, indem du als makroaktivierte Arbeitsmappe speicherst
                workbook.Save("temp.xlsm", SaveFormat.Xlsm);
                workbook = new Workbook("temp.xlsm");
                File.Delete("temp.xlsm");
            }

            // Füge ein neues Modul zum VBA‑Projekt hinzu
            int moduleIndex = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Hole das hinzugefügte Modul und setze dessen Code
            VbaModule module = workbook.VbaProject.Modules[moduleIndex];
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";

            // Speichere die Arbeitsmappe
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "VbaProjectDemo.xlsm");
            workbook.Save(outputPath, SaveFormat.Xlsm);
        }
    }
}
```

### Siehe auch

* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


