---
title: "Cells.ImportCSV"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Importiert eine CSV-Datei in die Zellen"
type: docs
url: /de/net/aspose.cells/cells/importcsv/
---
## ImportCSV(string, string, bool, int, int) {#importcsv_3}

Importiert eine CSV-Datei in die Zellen.

```csharp
public void ImportCSV(string fileName, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der CSV-Dateiname. |
| Splitter | String | Der Splitter |
| convertNumericData | Boolean | Ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Pfad zur CSV-Datei
            string csvPath = "example.csv";
            
            // CSV-Daten importieren, beginnend bei Zelle A1 (Zeile 0, Spalte 0)
            // Semikolon als Trennzeichen verwenden und numerische Daten konvertieren
            cells.ImportCSV(csvPath, ";", true, 0, 0);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, string, bool, int, int) {#importcsv_1}

Importiert eine CSV-Datei in die Zellen.

```csharp
public void ImportCSV(Stream stream, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der CSV-Datei-Stream. |
| Splitter | String | Der Splitter |
| convertNumericData | Boolean | Ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten für CSV im Speicher erstellen
            string csvData = "Name,Age,City\nJohn,30,New York\nAlice,25,London\nBob,35,Paris";
            byte[] byteArray = System.Text.Encoding.UTF8.GetBytes(csvData);
            MemoryStream csvStream = new MemoryStream(byteArray);

            try
            {
                // Rufen Sie die ImportCSV-Methode mit den Parametern Stream, String, Boolean, Int32, Int32 auf
                cells.ImportCSV(csvStream, ",", true, 0, 0);

                Console.WriteLine("CSV data imported successfully to worksheet.");
                Console.WriteLine($"Data range: A1 to {cells.MaxDisplayRange}");

                // Speichere die Arbeitsmappe
                workbook.Save("ImportCSVFromStreamDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                csvStream?.Dispose();
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(string, TxtLoadOptions, int, int) {#importcsv_2}

Importiert eine CSV-Datei in die Zellen.

```csharp
public void ImportCSV(string fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der CSV-Dateiname. |
| Optionen | TxtLoadOptions | Die Ladeoptionen zum Lesen der Textdatei |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // CSV-Ladeoptionen erstellen
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            loadOptions.ConvertDateTimeData = true;
            loadOptions.ConvertNumericData = true;
            loadOptions.ParsingFormulaOnOpen = true;

            // Beispielpfad zur CSV-Datei (durch den tatsächlichen Pfad in Ihrer Umgebung ersetzen)
            string csvFilePath = "example.csv";
            
            // CSV-Daten importieren, beginnend bei Zelle A1 (Zeile 0, Spalte 0)
            worksheet.Cells.ImportCSV(csvFilePath, loadOptions, 0, 0);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, TxtLoadOptions, int, int) {#importcsv}

Importiert eine CSV-Datei in die Zellen.

```csharp
public void ImportCSV(Stream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der CSV-Datei-Stream. |
| Optionen | TxtLoadOptions | Die Ladeoptionen zum Lesen der Textdatei |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Cells-Sammlung ab.
            Cells cells = worksheet.Cells;

            // Beispieldaten für CSV erstellen
            string csvData = "Name,Age,City\nJohn,30,New York\nJane,25,Los Angeles\nBob,35,Chicago";

            // Einen MemoryStream mit den CSV-Daten erstellen
            MemoryStream csvStream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData));

            try
            {
                // TxtLoadOptions für den CSV-Import erstellen
                TxtLoadOptions loadOptions = new TxtLoadOptions();
                loadOptions.Separator = ',';
                loadOptions.ConvertNumericData = true;

                // CSV-Daten importieren, beginnend bei Zeile 0, Spalte 0
                cells.ImportCSV(csvStream, loadOptions, 0, 0);

                // Speichere die Arbeitsmappe
                workbook.Save("ImportCSVDemo.xlsx");

                Console.WriteLine("CSV data imported successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                // Den Stream freigeben
                csvStream.Dispose();
            }
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


