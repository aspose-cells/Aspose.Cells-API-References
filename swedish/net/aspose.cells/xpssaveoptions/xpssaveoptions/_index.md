---
title: "XpsSaveOptions.XpsSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XpsSaveOptions-konstruktor. Skapar alternativ för att spara xps-fil"
type: docs
url: /sv/net/aspose.cells/xpssaveoptions/xpssaveoptions/
---
## XpsSaveOptions() {#constructor}

Skapar alternativ för att spara xps‑fil.

```csharp
public XpsSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XpsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("XPS Save Options Demo");

            // Initiera XpsSaveOptions med konstruktor
            XpsSaveOptions saveOptions = new XpsSaveOptions();

            // Konfigurera sparalternativ
            saveOptions.OnePagePerSheet = true;
            saveOptions.DefaultFont = "Arial";
            saveOptions.PageIndex = 0;
            saveOptions.PageCount = 1;

            // Spara arbetsbok med alternativ
            workbook.Save("XpsSaveOptionsDemo.xps", saveOptions);
        }
    }
}
```

### Se även

* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XpsSaveOptions(SaveFormat) {#constructor_1}

Skapar alternativ för att spara xps‑fil.

```csharp
[Obsolete("Use XpsSaveOptions() constructor instead.")]
public XpsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Sparaformatet måste vara xps-format. |

### Anmärkningar

OBS: Den här konstruktorn är nu föråldrad. Använd istället XpsSaveOptions()-konstruktorn. Denna egenskap kommer att tas bort 12 månader senare sedan augusti 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XpsSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "XPS Save Options Demo";
            worksheet.Cells["B1"].Value = "Using SaveFormat parameter";

            try
            {
                // Skapa XpsSaveOptions med konstruktorn och SaveFormat-parameter
                XpsSaveOptions saveOptions = new XpsSaveOptions(SaveFormat.Xps);

                // Spara arbetsboken med de angivna alternativen
                workbook.Save("XpsSaveOptionsWithSaveFormatDemo.xps", saveOptions);

                Console.WriteLine("XpsSaveOptions created successfully with SaveFormat parameter");
                Console.WriteLine("Workbook saved as XPS format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating XpsSaveOptions or saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


