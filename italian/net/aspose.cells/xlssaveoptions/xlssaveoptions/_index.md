---
title: "XlsSaveOptions.XlsSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore XlsSaveOptions. Crea le opzioni per salvare un file Excel 972003 xls"
type: docs
url: /it/net/aspose.cells/xlssaveoptions/xlssaveoptions/
---
## XlsSaveOptions() {#constructor}

Crea le opzioni per salvare il file Excel 97-2003 xls.

```csharp
public XlsSaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Sample XLS File");
            worksheet.Cells["A2"].PutValue("Created using XlsSaveOptions");

            // Inizializza XlsSaveOptions usando il costruttore
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            // Imposta alcune opzioni (rimosse le proprietà non supportate)
            saveOptions.IsTemplate = false;

            // Salva la cartella di lavoro con le opzioni
            workbook.Save("output.xls", saveOptions);

            Console.WriteLine("File saved successfully with XlsSaveOptions.");
        }
    }
}
```

### Vedi anche

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsSaveOptions(SaveFormat) {#constructor_1}

Crea le opzioni per salvare il file Excel 97-2003 xls/xlt.

```csharp
public XlsSaveOptions(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato del file. Dovrebbe essere Excel97To2003 o Xlt, altrimenti il formato salvato verrà impostato automaticamente su Excel97To2003. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);
            
            try
            {
                // Chiama il metodo #ctor con il parametro SaveFormat
                XlsSaveOptions saveOptions = new XlsSaveOptions(SaveFormat.Excel97To2003);
                
                // Imposta proprietà aggiuntive
                saveOptions.MatchColor = true;
                saveOptions.WpsCompatibility = false;
                
                Console.WriteLine("XlsSaveOptions constructor executed successfully with SaveFormat parameter");
                
                // Salva la cartella di lavoro con le opzioni specificate
                workbook.Save("XlsSaveOptionsCtorDemo.xls", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XlsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


