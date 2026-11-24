---
title: "TxtLoadOptions.TxtLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions Konstruktor. Erstellt die Optionen zum Laden einer Textdatei"
type: docs
url: /de/net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Erstellt die Optionen zum Laden einer Textdatei.

```csharp
public TxtLoadOptions()
```

### Hinweise

Der standardmäßige Lade-Dateityp ist CSV.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues TxtLoadOptions mit dem Konstruktor
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            
            // Setze Trennzeichen für CSV-Datei
            loadOptions.Separator = ',';
            
            // Erstelle Arbeitsmappe mit Ladeoptionen
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Gib einige Informationen aus der geladenen Datei aus
            Console.WriteLine("Worksheet count: " + workbook.Worksheets.Count);
            Console.WriteLine("First cell value: " + workbook.Worksheets[0].Cells["A1"].Value);
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Erstellt die Optionen zum Laden einer Textdatei.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadFormat | LoadFormat | Das Ladeformat |

### Beispiele

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
            // Erstelle Beispiel‑CSV‑Inhalt und temporäre Datei
            string csvData = "Column1,Column2,Column3\nData1,Data2,Data3";
            string tempFile = Path.GetTempFileName();
            File.WriteAllText(tempFile, csvData);

            try
            {
                // Erstelle TxtLoadOptions mit LoadFormat.Csv
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
                loadOptions.Separator = ',';
                loadOptions.HasTextQualifier = true;

                // Lade CSV mit den konfigurierten Optionen
                Workbook workbook = new Workbook(tempFile, loadOptions);
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstriere geladene Daten
                Console.WriteLine($"A1 Cell Value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 Cell Value: {worksheet.Cells["B2"].StringValue}");

                // Speichere verarbeitete Arbeitsmappe
                workbook.Save("TxtLoadOptionsCtorDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor: {ex.Message}");
            }
            finally
            {
                // Bereinige temporäre Datei
                if (File.Exists(tempFile))
                {
                    File.Delete(tempFile);
                }
            }
        }
    }
}
```

### Siehe auch

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


