---
title: "SaveOptions.WarningCallback"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Hämtar eller anger varningsåteranrop"
type: docs
url: /sv/net/aspose.cells/saveoptions/warningcallback/
---
## SaveOptions.WarningCallback property

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
    public class SaveOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data");

            // Skapa sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Ange anpassat varningsåteranrop
            saveOptions.WarningCallback = new CustomWarningCallback();

            // Detta kommer att generera en varning om en funktion som inte stöds i HTML-format
            worksheet.PageSetup.PrintTitleRows = "$1:$1";

            // Spara med alternativ som kan utlösa varningar
            workbook.Save("WarningCallbackDemo.html", saveOptions);
        }
    }

    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Hantera varningen - i detta fall bara visa den
            Console.WriteLine($"Warning: {warningInfo.Description}");
            Console.WriteLine($"Warning type: {warningInfo.WarningType}");
        }
    }
}
```

### Se även

* interface [IWarningCallback](../../iwarningcallback/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


