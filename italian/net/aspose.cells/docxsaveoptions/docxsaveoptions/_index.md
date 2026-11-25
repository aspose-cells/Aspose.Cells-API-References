---
title: "DocxSaveOptions.DocxSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore DocxSaveOptions. Rappresenta le opzioni di salvataggio di un file .docx"
type: docs
url: /it/net/aspose.cells/docxsaveoptions/docxsaveoptions/
---
## DocxSaveOptions() {#constructor}

Rappresenta le opzioni per il salvataggio del file .docx.

```csharp
public DocxSaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Inizializza DocxSaveOptions usando il costruttore
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            
            // Salva la cartella di lavoro come DOCX con le opzioni
            workbook.Save("output.docx", saveOptions);
            
            Console.WriteLine("Document saved successfully with DocxSaveOptions.");
        }
    }
}
```

### Vedi anche

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DocxSaveOptions(bool) {#constructor_1}

Rappresenta le opzioni per il salvataggio del file .docx.

```csharp
public DocxSaveOptions(bool saveAsImage)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveAsImage | Booleano | Se True, la cartella di lavoro verrà convertita in alcune immagini del file .docx. Se False, la cartella di lavoro verrà convertita in alcune tabelle del file .docx. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Salva come DOCX con le opzioni predefinite
            workbook.Save("output_default.docx");
            
            // Salva come DOCX con DocxSaveOptions(true) - ottimizzato per MS Word
            workbook.Save("output_optimized.docx", new DocxSaveOptions(true));
        }
    }
}
```

### Vedi anche

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


