---
title: "DocxSaveOptions.DocxSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocxSaveOptions‑Konstruktor. Stellt Optionen zum Speichern einer .docx‑Datei dar"
type: docs
url: /de/net/aspose.cells/docxsaveoptions/docxsaveoptions/
---
## DocxSaveOptions() {#constructor}

Stellt Optionen zum Speichern von .docx‑Dateien dar.

```csharp
public DocxSaveOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Initialisieren Sie DocxSaveOptions mit dem Konstruktor
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            
            // Speichern Sie die Arbeitsmappe als DOCX mit Optionen
            workbook.Save("output.docx", saveOptions);
            
            Console.WriteLine("Document saved successfully with DocxSaveOptions.");
        }
    }
}
```

### Siehe auch

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DocxSaveOptions(bool) {#constructor_1}

Stellt Optionen zum Speichern von .docx‑Dateien dar.

```csharp
public DocxSaveOptions(bool saveAsImage)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveAsImage | Boolean | Wenn True, wird die Arbeitsmappe in einige Bilder der .docx‑Datei konvertiert. Wenn False, wird die Arbeitsmappe in einige Tabellen der .docx‑Datei konvertiert. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Als DOCX mit Standardoptionen speichern
            workbook.Save("output_default.docx");
            
            // Als DOCX mit DocxSaveOptions(true) speichern – optimiert für MS Word
            workbook.Save("output_optimized.docx", new DocxSaveOptions(true));
        }
    }
}
```

### Siehe auch

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


