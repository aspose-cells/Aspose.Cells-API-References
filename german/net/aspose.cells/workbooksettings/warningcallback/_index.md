---
title: "WorkbookSettings.WarningCallback"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt den Warnungs-Callback zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/workbooksettings/warningcallback/
---
## WorkbookSettings.WarningCallback property

Liest oder setzt den Warnungs-Callback.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Setzt den Warn‑Callback
            workbook.Settings.WarningCallback = new WarningCallbackImplementation();

            // Erstelle ein Arbeitsblatt mit einem potenziellen Warnungsfall (doppelter benannter Bereich)
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test");
            
            // Dies löst eine Warnung über einen doppelten Namen aus
            int index1 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1";

            // Speichere die Arbeitsmappe (löst den Warnungs-Callback aus)
            workbook.Save("WarningCallbackExample.xlsx");
        }
    }

    public class WarningCallbackImplementation : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.WarningType}, Description: {warningInfo.Description}");
        }
    }
}
```

### Siehe auch

* interface [IWarningCallback](../../iwarningcallback/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


