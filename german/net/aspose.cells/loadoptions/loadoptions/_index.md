---
title: "LoadOptions.LoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions‑Konstruktor. Erstellt Optionen zum Laden der Datei"
type: docs
url: /de/net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Erstellt eine Option zum Laden der Datei.

```csharp
public LoadOptions()
```

### Beispiele

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
                // Erstelle Beispiel‑CSV‑Inhalt
                File.WriteAllText(tempCsvPath, "Name,Age\nJohn,30\nJane,25");

                // Standard‑Konstruktor demonstrieren
                LoadOptions defaultOptions = new LoadOptions();
                Console.WriteLine("Default LoadFormat: " + defaultOptions.LoadFormat);

                // Konstruktor mit LoadFormat‑Parameter demonstrieren
                LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
                Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

                // CSV-Datei mit den angegebenen Optionen laden
                Workbook workbook = new Workbook(tempCsvPath, csvOptions);

                // Verifizieren, dass die Daten korrekt geladen wurden
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"Cell A1: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"Cell B2: {worksheet.Cells["B2"].StringValue}");

                // Als XLSX speichern, um die Konvertierung zu demonstrieren
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

### Siehe auch

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

Erstellt eine Option zum Laden der Datei.

```csharp
public LoadOptions(LoadFormat loadFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadFormat | LoadFormat | Das Ladeformat. |

### Beispiele

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
                // Erstelle Beispiel‑CSV‑Inhalt
                File.WriteAllText(tempCsvPath, "Column1,Column2\nData1,Data2");

                // LoadOptions mit LoadFormat.Csv erstellen
                LoadOptions options = new LoadOptions(LoadFormat.Csv);

                // CSV-Datei mit den erstellten Optionen laden
                Workbook workbook = new Workbook(tempCsvPath, options);

                // Erfolgreiches Laden demonstrieren, indem die Zelle gelesen wird
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"A1 cell value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 cell value: {worksheet.Cells["B2"].StringValue}");

                // Als XLSX speichern, um die Konvertierungsfähigkeit zu zeigen
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

### Siehe auch

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


