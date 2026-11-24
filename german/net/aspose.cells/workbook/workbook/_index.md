---
title: "Workbook.Workbook"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Konstruktor. Initialisiert eine neue Instanz der Workbook-Klasse"
type: docs
url: /de/net/aspose.cells/workbook/workbook/
---
## Workbook() {#constructor}

Initialisiert eine neue Instanz der [`Workbook`](../)-Klasse.

```csharp
public Workbook()
```

### Hinweise

Der Standard-Dateiformattyp ist Xlsx. Wenn Sie andere Dateitypen erstellen möchten, verwenden Sie bitte Workbook(FileFormatType).

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit dem Konstruktor
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorkbookCtorDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(FileFormatType) {#constructor_1}

Initialisiert eine neue Instanz der [`Workbook`](../)-Klasse.

```csharp
public Workbook(FileFormatType fileFormatType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileFormatType | FileFormatType | Das neue Dateiformat. |

### Hinweise

Der Standard-Dateiformattyp ist Excel97To2003.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit dem XLSX-Dateiformat
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Daten in Zelle A1 ein
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(LoadOptions) {#constructor_2}

Initialisiert eine neue leere Instanz der [`Workbook`](../)-Klasse mit Optionen

```csharp
public Workbook(LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | LoadOptions | Die Optionen. |

### Siehe auch

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string) {#constructor_5}

Initialisiert eine neue Instanz der [`Workbook`](../)-Klasse und öffnet eine Datei.

```csharp
public Workbook(string file)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| file | String | Der Dateiname. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Der Pfad zum Dokumentenverzeichnis.
            string dataDir = "Your Document Directory";

            // Erstelle eine Arbeitsmappe aus einer vorhandenen Excel-Datei
            Workbook workbook = new Workbook(dataDir + "example.xlsx");

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Zeige einige Arbeitsblattinformationen an
            Console.WriteLine("Worksheet Name: " + worksheet.Name);
            Console.WriteLine("Number of Cells: " + worksheet.Cells.Count);

            // Speichere die Arbeitsmappe im MHTML-Format
            workbook.Save(dataDir + "output.mht", SaveFormat.MHtml);

            // Erstelle eine weitere Arbeitsmappe aus der gespeicherten MHTML-Datei
            Workbook workbook2 = new Workbook(dataDir + "output.mht");
            Console.WriteLine("Number of Worksheets in MHTML: " + workbook2.Worksheets.Count);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream) {#constructor_3}

Initialisiert eine neue Instanz der [`Workbook`](../)-Klasse und öffnet einen Stream.

```csharp
public Workbook(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Stream. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispiel-Excel-Datei im Speicher
            MemoryStream sampleStream = new MemoryStream();
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].Value = "Sample Data";
            sampleWorkbook.Save(sampleStream, SaveFormat.Xlsx);
            sampleStream.Position = 0; // Reset stream position for reading

            try
            {
                // Erstelle eine neue Workbook-Instanz mit dem Stream-Konstruktor
                Workbook workbook = new Workbook(sampleStream);

                // Greife auf das erste Arbeitsblatt zu
                Worksheet worksheet = workbook.Worksheets[0];

                // Zeige die geladenen Daten an
                Console.WriteLine($"Loaded data from stream: {worksheet.Cells["A1"].StringValue}");

                // Speichere die Arbeitsmappe in einer Datei
                workbook.Save("WorkbookFromStream.xlsx");
                Console.WriteLine("Workbook saved successfully from stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook from stream: {ex.Message}");
            }
            finally
            {
                sampleStream.Dispose();
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string, LoadOptions) {#constructor_6}

Initialisiert eine neue Instanz der [`Workbook`](../)-Klasse und öffnet eine Datei.

```csharp
public Workbook(string file, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| file | String | Der Dateiname. |
| loadOptions | LoadOptions | Die Ladeoptionen |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringLoadOptionsDemo
    {
        public static void Run()
        {
            // Erstelle Ladeoptionen ohne LightCellsDataHandler
            LoadOptions loadOptions = new LoadOptions();

            // Initialisiere das Workbook mit Dateipfad und Ladeoptionen
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Zeige, dass das Workbook geladen ist, indem die Arbeitsblattanzahl abgerufen wird
            Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream, LoadOptions) {#constructor_4}

Initialisiert eine neue Instanz der [`Workbook`](../)-Klasse und öffnet den Stream.

```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Stream. |
| loadOptions | LoadOptions | Die Ladeoptionen |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamLoadOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine Beispiel-Excel-Datei im Speicher
                byte[] sampleExcelData = GetSampleExcelData();
                MemoryStream stream = new MemoryStream(sampleExcelData);

                // Erstelle LoadOptions mit spezifischen Einstellungen
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.MemorySetting = MemorySetting.MemoryPreference;

                // Erstelle eine Workbook-Instanz mit dem #ctor unter Verwendung von Stream und LoadOptions
                Workbook workbook = new Workbook(stream, loadOptions);

                // Zeige grundlegende Informationen über das geladene Workbook an
                Console.WriteLine("Workbook loaded successfully!");
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
                Console.WriteLine("File format: " + workbook.FileFormat);

                // Greife auf das erste Arbeitsblatt zu
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine("First worksheet name: " + worksheet.Name);

                // Zeige einige Zellinhalte an, falls verfügbar
                if (worksheet.Cells["A1"].Value != null)
                {
                    Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value.ToString());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook: {ex.Message}");
            }
        }

        private static byte[] GetSampleExcelData()
        {
            // Erstelle eine einfache Excel-Datei im Speicher zur Demonstration
            using (MemoryStream ms = new MemoryStream())
            {
                Workbook tempWorkbook = new Workbook();
                tempWorkbook.Worksheets[0].Cells["A1"].PutValue("Sample Data");
                tempWorkbook.Worksheets[0].Cells["B1"].PutValue("Created for demo");
                tempWorkbook.Save(ms, SaveFormat.Xlsx);
                return ms.ToArray();
            }
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


