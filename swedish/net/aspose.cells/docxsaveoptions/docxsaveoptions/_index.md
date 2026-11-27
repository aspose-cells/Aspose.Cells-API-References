---
title: "DocxSaveOptions.DocxSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocxSaveOptions-konstruktor. Representerar alternativ för att spara .docx-fil"
type: docs
url: /sv/net/aspose.cells/docxsaveoptions/docxsaveoptions/
---
## DocxSaveOptions() {#constructor}

Representerar alternativ för att spara .docx-fil.

```csharp
public DocxSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Initiera DocxSaveOptions med hjälp av konstruktorn
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            
            // Spara arbetsboken som DOCX med alternativ
            workbook.Save("output.docx", saveOptions);
            
            Console.WriteLine("Document saved successfully with DocxSaveOptions.");
        }
    }
}
```

### Se även

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DocxSaveOptions(bool) {#constructor_1}

Representerar alternativ för att spara .docx-fil.

```csharp
public DocxSaveOptions(bool saveAsImage)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveAsImage | Boolean | Om True konverteras arbetsboken till några bilder i .docx-filen. Om False konverteras arbetsboken till några tabeller i .docx-filen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Spara som DOCX med standardalternativ
            workbook.Save("output_default.docx");
            
            // Spara som DOCX med DocxSaveOptions(true) - optimerad för MS Word
            workbook.Save("output_optimized.docx", new DocxSaveOptions(true));
        }
    }
}
```

### Se även

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


