---
title: "Cell.StringValueWithoutFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Ottiene il valore della cella come stringa senza alcun formato"
type: docs
url: /it/net/aspose.cells/cell/stringvaluewithoutformat/
---
## Cell.StringValueWithoutFormat property

Ottiene il valore della cella come stringa senza alcun formato.

```csharp
[Obsolete("Use GetStringValue(CellValueFormatStrategy) with CellValueFormatStrategy.None instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValueWithoutFormat { get; }
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, l'utente dovrebbe ottenere l'oggetto valore e formattarlo secondo il tipo di valore e i requisiti specifici. Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2020. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyStringValueWithoutFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi diversi tipi di dati per dimostrare StringValueWithoutFormat
            worksheet.Cells["A1"].PutValue("Plain Text");
            worksheet.Cells["A2"].PutValue(12345);
            worksheet.Cells["A3"].PutValue(3.14159);
            worksheet.Cells["A4"].PutValue(DateTime.Now);

            // Applica la formattazione numerica a alcune celle
            Style style = worksheet.Cells["A2"].GetStyle();
            style.Number = 3; // Currency format
            worksheet.Cells["A2"].SetStyle(style);

            style = worksheet.Cells["A3"].GetStyle();
            style.Number = 9; // Percentage format
            worksheet.Cells["A3"].SetStyle(style);

            try
            {
                // Visualizza StringValueWithoutFormat per ogni cella
                Console.WriteLine("A1 StringValueWithoutFormat: " + worksheet.Cells["A1"].StringValueWithoutFormat);
                Console.WriteLine("A2 StringValueWithoutFormat: " + worksheet.Cells["A2"].StringValueWithoutFormat);
                Console.WriteLine("A3 StringValueWithoutFormat: " + worksheet.Cells["A3"].StringValueWithoutFormat);
                Console.WriteLine("A4 StringValueWithoutFormat: " + worksheet.Cells["A4"].StringValueWithoutFormat);

                // Confronta con StringValue formattato
                Console.WriteLine("\nComparison with formatted values:");
                Console.WriteLine("A2 StringValue (formatted): " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3 StringValue (formatted): " + worksheet.Cells["A3"].StringValue);

                // Salva la cartella di lavoro
                workbook.Save("StringValueWithoutFormatDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


