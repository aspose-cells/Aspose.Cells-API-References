---
title: "XmlLoadOptions.XmlLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore XmlLoadOptions. Rappresenta le opzioni di caricamento del file xml"
type: docs
url: /it/net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

Rappresenta le opzioni di caricamento del file XML.

```csharp
public XmlLoadOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea nuove opzioni di caricamento XML
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Imposta per convertire valori numerici o di data
            options.ConvertNumericOrDate = true;
            
            // Carica la cartella di lavoro con opzioni
            Workbook workbook = new Workbook("input.xml", options);
            
            // Accedi ai dati della cella
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell Value: " + cell.Value);
            Console.WriteLine("Cell Type: " + cell.Type);
            
            // Salva cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

Rappresenta le opzioni di caricamento del file XML.

```csharp
public XmlLoadOptions(LoadFormat type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | LoadFormat | Il tipo di formato di caricamento. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza di XmlLoadOptions con il parametro LoadFormat
                LoadFormat loadFormat = LoadFormat.Xml;
                XmlLoadOptions xmlLoadOptions = new XmlLoadOptions(loadFormat);

                // Imposta alcune proprietà di XmlLoadOptions
                xmlLoadOptions.StartCell = "A1";
                xmlLoadOptions.IsXmlMap = true;
                xmlLoadOptions.ConvertNumericOrDate = true;

                // Crea una cartella di lavoro usando le opzioni di caricamento
                Workbook workbook = new Workbook("sample.xml", xmlLoadOptions);

                // Accedi al primo foglio di lavoro
                Worksheet worksheet = workbook.Worksheets[0];

                // Visualizza alcune informazioni
                Console.WriteLine("XML file loaded successfully with LoadFormat.Xml");
                Console.WriteLine($"First cell value: {worksheet.Cells["A1"].Value}");

                // Salva la cartella di lavoro
                workbook.Save("XmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XmlLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


