---
title: "OoxmlSaveOptions.OoxmlSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore OoxmlSaveOptions. Crea le opzioni per salvare un file Office Open XML"
type: docs
url: /it/net/aspose.cells/ooxmlsaveoptions/ooxmlsaveoptions/
---
## OoxmlSaveOptions() {#constructor}

Crea le opzioni per salvare un file Office Open XML.

```csharp
public OoxmlSaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi alcuni dati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Dimostra il costruttore OoxmlSaveOptions
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            
            // Salva la cartella di lavoro con le opzioni OOXML
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML options.");
        }
    }
}
```

### Vedi anche

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OoxmlSaveOptions(SaveFormat) {#constructor_1}

Crea le opzioni per salvare un file Office Open XML.

```csharp
public OoxmlSaveOptions(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato file. Deve essere uno dei seguenti tipi: Xlsx, Xltx, Xlam, Xlsm o Xltm, altrimenti il formato salvato verrà impostato automaticamente su Xlsx. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            try
            {
                // Crea OoxmlSaveOptions con il parametro SaveFormat
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                
                // Imposta alcune proprietà delle opzioni di salvataggio
                saveOptions.ExportCellName = true;
                saveOptions.CompressionType = OoxmlCompressionType.Level6;
                
                Console.WriteLine("OoxmlSaveOptions created successfully with SaveFormat.Xlsx");
                
                // Salva la cartella di lavoro con le opzioni specificate
                workbook.Save("OoxmlSaveOptionsCtorDemo.xlsx", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating OoxmlSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


