---
title: "SpreadsheetML2003SaveOptions.IsIndentedFormatting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SpreadsheetML2003SaveOptions. Fa sì che gli elementi figlio siano indentati"
type: docs
url: /it/net/aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/
---
## SpreadsheetML2003SaveOptions.IsIndentedFormatting property

Fa sì che gli elementi figli siano indentati.

```csharp
public bool IsIndentedFormatting { get; set; }
```

### Osservazioni

Il valore predefinito è true. Se il valore è false, ridurrà la dimensione del file xml

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyIsIndentedFormattingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Configura le opzioni di salvataggio con formattazione indentata
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions
            {
                IsIndentedFormatting = true
            };

            // Salva con formattazione XML indentata
            workbook.Save("output_indented.xml", saveOptions);

            // Salva senza formattazione indentata per confronto
            saveOptions.IsIndentedFormatting = false;
            workbook.Save("output_not_indented.xml", saveOptions);
        }
    }
}
```

### Vedi anche

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


