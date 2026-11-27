---
title: "XlsbSaveOptions.XlsbSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XlsbSaveOptions-konstruktor. Skapar sparalternativ för xlsb-fil"
type: docs
url: /sv/net/aspose.cells/xlsbsaveoptions/xlsbsaveoptions/
---
## XlsbSaveOptions() {#constructor}

Skapar alternativ för att spara xlsb‑fil.

```csharp
public XlsbSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Test Value");

            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.ExportAllColumnIndexes = true;

            workbook.Save("output.xlsb", saveOptions);
        }
    }
}
```

### Se även

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsbSaveOptions(SaveFormat) {#constructor_1}

Skapar alternativ för att spara xlsb‑fil.

```csharp
[Obsolete("Use XlsbSaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public XlsbSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Sparaformatet . Det måste vara xlsb. |

### Anmärkningar

OBS: Denna konstruktor är nu föråldrad. Använd istället XlsbSaveOptions()-konstruktorn. Denna egenskap kommer att tas bort 12 månader senare sedan januari 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsbSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Using XlsbSaveOptions";

            try
            {
                // Skapa XlsbSaveOptions med konstruktorn som har SaveFormat-parameter
                XlsbSaveOptions saveOptions = new XlsbSaveOptions(SaveFormat.Xlsb);

                // Ange ytterligare egenskaper om det behövs
                saveOptions.ExportAllColumnIndexes = true;

                // Spara arbetsboken med de angivna sparalternativen
                workbook.Save("XlsbSaveOptionsDemo.xlsb", saveOptions);

                Console.WriteLine("Workbook saved successfully with XlsbSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


