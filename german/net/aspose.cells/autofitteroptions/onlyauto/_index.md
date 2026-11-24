---
title: "AutoFitterOptions.OnlyAuto"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFitterOptions-Eigenschaft. Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist."
type: docs
url: /de/net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist.

```csharp
public bool OnlyAuto { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyOnlyAutoDemo
    {
        public static void Run()
        {
            // Ladeoptionen erstellen und OnlyAuto-Eigenschaft festlegen
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = new AutoFitterOptions();
            loadOptions.AutoFitterOptions.OnlyAuto = true;

            // Arbeitsmappe mit Auto-Fit-Optionen laden
            Workbook workbook = new Workbook("example.xml", loadOptions);
            
            // Demonstriere Auto-Anpassung, indem die Spaltenbreite überprüft wird
            Console.WriteLine("Column width after auto-fit: " + 
                workbook.Worksheets[0].Cells.GetColumnWidthPixel(0));
            
            // Speichern und neu laden, um die Persistenz zu überprüfen
            workbook.Save("example_output.xlsx");
            Workbook reloaded = new Workbook("example_output.xlsx");
            Console.WriteLine("Reloaded column width: " + 
                reloaded.Worksheets[0].Cells.GetColumnWidthPixel(0));
        }
    }
}
```

### Siehe auch

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


