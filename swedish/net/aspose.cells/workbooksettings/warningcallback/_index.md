---
title: "WorkbookSettings.WarningCallback"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Hämtar eller anger varningsåteranrop"
type: docs
url: /sv/net/aspose.cells/workbooksettings/warningcallback/
---
## WorkbookSettings.WarningCallback property

Hämtar eller anger varningsåteranrop.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in varningsåteruppringning
            workbook.Settings.WarningCallback = new WarningCallbackImplementation();

            // Skapa ett kalkylblad med ett potentiellt varningsscenario (duplicerat namngivet område)
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test");
            
            // Detta kommer att utlösa en varning om duplicerat namn
            int index1 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1";

            // Spara arbetsboken (kommer att utlösa varningsåteranrop)
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

### Se även

* interface [IWarningCallback](../../iwarningcallback/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


