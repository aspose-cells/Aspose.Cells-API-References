---
title: "SpreadsheetML2003SaveOptions.SpreadsheetML2003SaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpreadsheetML2003SaveOptions-konstruktor. Skapar alternativ för att spara Excel 2003 spreadml-fil"
type: docs
url: /sv/net/aspose.cells/spreadsheetml2003saveoptions/spreadsheetml2003saveoptions/
---
## SpreadsheetML2003SaveOptions() {#constructor}

Skapar alternativen för att spara Excel 2003‑spreadml‑fil.

```csharp
public SpreadsheetML2003SaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet och lägg till exempeldata.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Skapa SpreadsheetML2003SaveOptions med konstruktor
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            
            // Ställ in alternativ
            saveOptions.LimitAsXls = true;
            saveOptions.ExportColumnIndexOfCell = true;

            // Spara med alternativen
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with SpreadsheetML2003SaveOptions");
        }
    }
}
```

### Se även

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SpreadsheetML2003SaveOptions(SaveFormat) {#constructor_1}

Skapar alternativen för att spara Excel 2003‑spreadml‑fil.

```csharp
[Obsolete("Use SpreadsheetML2003SaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SpreadsheetML2003SaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Sparaformatet. |

### Anmärkningar

OBS: Den här konstruktorn är nu föråldrad. Använd istället SpreadsheetML2003SaveOptions() konstruktorn. Denna egenskap kommer att tas bort 12 månader senare sedan januari 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SpreadsheetML2003SaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);

            try
            {
                // Anropa #ctor‑metoden med SaveFormat‑parameter
                SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();

                // Ställ in några egenskaper för sparalternativen
                saveOptions.IsIndentedFormatting = true;
                saveOptions.LimitAsXls = false;
                saveOptions.ExportColumnIndexOfCell = true;

                Console.WriteLine("SpreadsheetML2003SaveOptions created successfully with SaveFormat parameter");

                // Spara arbetsboken med de skapade sparalternativen
                workbook.Save("SpreadsheetML2003Output.xml", saveOptions);
                Console.WriteLine("Workbook saved successfully with SpreadsheetML2003SaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SpreadsheetML2003SaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


