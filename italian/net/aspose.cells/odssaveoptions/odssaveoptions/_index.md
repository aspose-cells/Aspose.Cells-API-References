---
title: "OdsSaveOptions.OdsSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore OdsSaveOptions. Crea le opzioni per il salvataggio del file ods"
type: docs
url: /it/net/aspose.cells/odssaveoptions/odssaveoptions/
---
## OdsSaveOptions() {#constructor}

Crea le opzioni di salvataggio del file ods.

```csharp
public OdsSaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi celle di esempio con diversi stili di bordo
            worksheet.Cells["B2"].PutValue("Medium Border");
            worksheet.Cells["B4"].PutValue("Thick Border");
            worksheet.Cells["B7"].PutValue("Double Border");
            
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Medium;
            worksheet.Cells["B2"].SetStyle(style);
            
            style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            worksheet.Cells["B4"].SetStyle(style);
            
            style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            worksheet.Cells["B7"].SetStyle(style);

            // Dimostra il costruttore OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
            
            // Salva come file ODS
            workbook.Save("output.ods", saveOptions);
            
            Console.WriteLine("File saved with OdsSaveOptions constructor demo.");
        }
    }
}
```

### Vedi anche

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsSaveOptions(SaveFormat) {#constructor_1}

Crea le opzioni di salvataggio del file ods.

```csharp
public OdsSaveOptions(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato del file. Deve essere Ods, Ots, Fods o Sxc, altrimenti il formato salvato verrà impostato automaticamente su Ods. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsSaveOptionsMethodCtorWithSaveFormatDemo
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
                OdsSaveOptions saveOptions = new OdsSaveOptions(SaveFormat.Ods);
                
                // Imposta alcune proprietà delle opzioni di salvataggio
                saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
                saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
                
                Console.WriteLine("OdsSaveOptions constructor executed successfully with SaveFormat.Ods parameter");
                
                // Salva la cartella di lavoro con le opzioni specificate
                workbook.Save("OdsSaveOptionsCtorDemo.ods", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OdsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


