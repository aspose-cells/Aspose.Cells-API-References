---
title: "Workbook.Save"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Speichert das Arbeitsbuch auf die Festplatte"
type: docs
url: /de/net/aspose.cells/workbook/save/
---
## Save(string, SaveFormat) {#save_3}

Speichert die Arbeitsmappe auf der Festplatte.

```csharp
public void Save(string fileName, SaveFormat saveFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der Dateiname. |
| saveFormat | SaveFormat | Der Speicherformattyp. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Speichern Sie das Arbeitsbuch im XLSX-Format
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Speichern Sie das Arbeitsbuch im PDF-Format
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string) {#save_2}

Speichert die Arbeitsmappe auf der Festplatte.

```csharp
public void Save(string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Speichern Sie das Arbeitsbuch in verschiedenen Formaten mithilfe eines Zeichenkettenparameters
            workbook.Save("output.xlsx");
            workbook.Save("output.xls");
            workbook.Save("output.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string, SaveOptions) {#save_4}

Speichert die Arbeitsmappe auf der Festplatte.

```csharp
public void Save(string fileName, SaveOptions saveOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der Dateiname. |
| saveOptions | SaveOptions | Die Speicheroptionen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // HTML-Speicheroptionen erstellen und konfigurieren
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Arbeitsmappe mit Optionen speichern
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("Workbook saved successfully with HTML options.");
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveFormat) {#save}

Speichert die Arbeitsmappe in den Stream.

```csharp
public void Save(Stream stream, SaveFormat saveFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Dateistream. |
| saveFormat | SaveFormat | Der Dateiformattyp zum Speichern. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            try
            {
                // Erstelle einen MemoryStream, um die Arbeitsmappe zu speichern
                using (MemoryStream stream = new MemoryStream())
                {
                    // Speichere die Arbeitsmappe im Stream im XLSX-Format
                    workbook.Save(stream, SaveFormat.Xlsx);

                    // Erfolgsmeldung anzeigen
                    Console.WriteLine("Workbook saved to stream successfully in XLSX format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Setze die Stream-Position zurück für mögliche weitere Verarbeitung
                    stream.Position = 0;

                    // Optional in eine Datei speichern zur Überprüfung
                    using (FileStream fileStream = File.Create("StreamSaveDemo.xlsx"))
                    {
                        stream.CopyTo(fileStream);
                    }
                    Console.WriteLine("Stream content also saved to file: StreamSaveDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook to stream: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveOptions) {#save_1}

Speichert die Arbeitsmappe in den Stream.

```csharp
public void Save(Stream stream, SaveOptions saveOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Dateistream. |
| saveOptions | SaveOptions | Die Speicheroptionen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Hello, Aspose.Cells!";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            // Erstelle einen MemoryStream, um die Arbeitsmappe zu speichern
            MemoryStream stream = new MemoryStream();

            try
            {
                // Erstelle SaveOptions für das PDF-Format
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Speichere die Arbeitsmappe im Stream mit den angegebenen Optionen
                workbook.Save(stream, saveOptions);

                Console.WriteLine("Workbook saved to stream successfully in PDF format.");
                Console.WriteLine($"Stream length: {stream.Length} bytes");

                // Setze die Stream-Position zurück für mögliche weitere Verwendung
                stream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
            finally
            {
                // Ressourcen bereinigen
                stream?.Dispose();
                workbook?.Dispose();
            }
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions) {#save_5}

Erstellt die Ergebnis-Tabelle und überträgt sie an den Client, dann öffnet sie im Browser oder in MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Antwort | HttpResponse | Response-Objekt, um die Tabelle an den Client zurückzugeben. |
| fileName | String | Der Name der erstellten Datei. |
| contentDisposition | ContentDisposition | Der Typ der Inhalts‑Disposition. |
| saveOptions | SaveOptions | Die Speicheroptionen. |

### Hinweise

Diese Methode ist nur für net4.x-Versionen verfügbar.

### Siehe auch

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions, bool) {#save_6}

Erstellt die Ergebnis-Tabelle und überträgt sie an den Client, dann öffnet sie im Browser oder in MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions, bool enableHttpCompression)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Antwort | HttpResponse | Response-Objekt, um die Tabelle an den Client zurückzugeben. |
| fileName | String | Der Name der erstellten Datei. |
| contentDisposition | ContentDisposition | Der Typ der Inhalts‑Disposition. |
| saveOptions | SaveOptions | Die Speicheroptionen. |
| enableHttpCompression | Boolean | Ob HTTP-Komprimierung verwendet werden soll |

### Hinweise

Diese Methode ist nur für net4.x-Versionen verfügbar.

### Siehe auch

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


