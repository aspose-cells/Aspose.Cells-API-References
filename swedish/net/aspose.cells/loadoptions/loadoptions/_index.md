---
title: "LoadOptions.LoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions‑konstruktor. Skapar ett alternativ för att läsa in filen"
type: docs
url: /sv/net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Skapar alternativ för att läsa in filen.

```csharp
public LoadOptions()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";

            try
            {
                // Skapa exempel-CSV-innehåll
                File.WriteAllText(tempCsvPath, "Name,Age\nJohn,30\nJane,25");

                // Demonstrera standardkonstruktorn
                LoadOptions defaultOptions = new LoadOptions();
                Console.WriteLine("Default LoadFormat: " + defaultOptions.LoadFormat);

                // Demonstrera konstruktor med LoadFormat‑parameter
                LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
                Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

                // Läs in CSV‑fil med de angivna alternativen
                Workbook workbook = new Workbook(tempCsvPath, csvOptions);

                // Verifiera att data har lästs in korrekt
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"Cell A1: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"Cell B2: {worksheet.Cells["B2"].StringValue}");

                // Spara som XLSX för att demonstrera konvertering
                workbook.Save("CsvToExcel.xlsx");
                Console.WriteLine("CSV file successfully loaded and converted to XLSX");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

Skapar alternativ för att läsa in filen.

```csharp
public LoadOptions(LoadFormat loadFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadFormat | LoadFormat | Laddningsformatet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";
            
            try
            {
                // Skapa exempel-CSV-innehåll
                File.WriteAllText(tempCsvPath, "Column1,Column2\nData1,Data2");

                // Skapa LoadOptions med LoadFormat.Csv
                LoadOptions options = new LoadOptions(LoadFormat.Csv);

                // Läs in CSV‑fil med de skapade alternativen
                Workbook workbook = new Workbook(tempCsvPath, options);

                // Demonstrera lyckad inläsning genom att läsa en cell
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"A1 cell value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 cell value: {worksheet.Cells["B2"].StringValue}");

                // Spara som XLSX för att visa konverteringsmöjlighet
                workbook.Save("CsvLoadedAsExcel.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during CSV loading: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### Se även

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


