---
title: "TxtLoadOptions.TxtLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions-konstruktör. Skapar alternativ för att läsa in textfil"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Skapar alternativen för att läsa in textfil.

```csharp
public TxtLoadOptions()
```

### Anmärkningar

Standardfiltypen för inläsning är CSV.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa ny TxtLoadOptions med hjälp av konstruktören
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            
            // Ange separator för CSV-fil
            loadOptions.Separator = ',';
            
            // Skapa arbetsbok med inläsningsalternativ
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Skriv ut viss information från den inlästa filen
            Console.WriteLine("Worksheet count: " + workbook.Worksheets.Count);
            Console.WriteLine("First cell value: " + workbook.Worksheets[0].Cells["A1"].Value);
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Skapar alternativen för att läsa in textfil.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadFormat | LoadFormat | Laddningsformatet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class TxtLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Skapa exempel på CSV-innehåll och en tillfällig fil
            string csvData = "Column1,Column2,Column3\nData1,Data2,Data3";
            string tempFile = Path.GetTempFileName();
            File.WriteAllText(tempFile, csvData);

            try
            {
                // Skapa TxtLoadOptions med LoadFormat.Csv
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
                loadOptions.Separator = ',';
                loadOptions.HasTextQualifier = true;

                // Läs in CSV med de konfigurerade alternativen
                Workbook workbook = new Workbook(tempFile, loadOptions);
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstrera inlästa data
                Console.WriteLine($"A1 Cell Value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 Cell Value: {worksheet.Cells["B2"].StringValue}");

                // Spara bearbetad arbetsbok
                workbook.Save("TxtLoadOptionsCtorDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor: {ex.Message}");
            }
            finally
            {
                // Rensa upp tillfällig fil
                if (File.Exists(tempFile))
                {
                    File.Delete(tempFile);
                }
            }
        }
    }
}
```

### Se även

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


