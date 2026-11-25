---
title: "PivotTableFormat.GetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTableFormat. Restituisce lo stile formattato"
type: docs
url: /it/net/aspose.cells.pivot/pivottableformat/getstyle/
---
## PivotTableFormat.GetStyle method

Ottiene lo stile formattato.

```csharp
public Style GetStyle()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableFormatMethodGetStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ottieni il formato della tabella pivot
            PivotTableFormatCollection formats = pivotTable.PivotFormats;
            PivotTableFormat format = formats[0];

            try
            {
                // Chiama il metodo GetStyle
                Style style = format.GetStyle();

                // Proprietà dello stile di visualizzazione
                Console.WriteLine("Style properties:");
                Console.WriteLine($"Font Name: {style.Font.Name}");
                Console.WriteLine($"Font Size: {style.Font.Size}");
                Console.WriteLine($"Background Color: {style.BackgroundColor}");

                // Modifica lo stile
                style.Font.Name = "Arial";
                style.Font.Size = 12;
                style.BackgroundColor = System.Drawing.Color.LightBlue;

                // Applica lo stile modificato nuovamente al formato
                format.SetStyle(style);

                Console.WriteLine("GetStyle method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStyle method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("PivotTableFormatMethodGetStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


