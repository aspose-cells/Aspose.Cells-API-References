---
title: "LoadOptions.LoadFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Der Filter, der angibt, wie Daten geladen werden sollen"
type: docs
url: /de/net/aspose.cells/loadoptions/loadfilter/
---
## LoadOptions.LoadFilter property

Der Filter, der angibt, wie Daten geladen werden.

```csharp
public LoadFilter LoadFilter { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomLoadFilter : LoadFilter
    {
        public override void StartSheet(Worksheet sheet)
        {
            // Daten nur laden, wenn das Blatt sichtbar ist
            if (sheet.IsVisible)
            {
                base.StartSheet(sheet);
            }
        }
    }

    public class LoadOptionsPropertyLoadFilterDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Testarbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "HiddenSheet";
            sheet.IsVisible = false;
            sheet.Cells["A1"].PutValue("This should not load");
            
            // Fügen Sie ein sichtbares Blatt hinzu
            Worksheet visibleSheet = workbook.Worksheets.Add("VisibleSheet");
            visibleSheet.Cells["A1"].PutValue("This will load");
            
            // Speichern Sie die Testdatei
            string filePath = "LoadFilterTest.xlsx";
            workbook.Save(filePath);
            workbook.Dispose();

            // Mit benutzerdefiniertem Filter laden
            LoadOptions options = new LoadOptions();
            options.LoadFilter = new CustomLoadFilter();
            
            Workbook loadedWorkbook = new Workbook(filePath, options);
            
            // Überprüfen Sie, dass nur das sichtbare Blatt geladen wurde
            Console.WriteLine("Loaded Sheets:");
            foreach (Worksheet ws in loadedWorkbook.Worksheets)
            {
                Console.WriteLine($"- {ws.Name}: Visible={ws.IsVisible}");
                if (ws.IsVisible)
                {
                    Console.WriteLine($"  A1 Value: {ws.Cells["A1"].StringValue}");
                }
            }
            
            loadedWorkbook.Dispose();
        }
    }
}
```

### Siehe auch

* class [LoadFilter](../../loadfilter/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


