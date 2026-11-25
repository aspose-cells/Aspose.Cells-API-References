---
title: "Column.GetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Column. Ottiene lo stile di questa colonna"
type: docs
url: /it/net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

Restituisce lo stile di questa colonna.

```csharp
public Style GetStyle()
```

### Osservazioni

Modificare direttamente l'oggetto stile restituito non ha effetto per questa colonna o per le celle in questa colonna. È necessario chiamare il metodo [`ApplyStyle`](../applystyle/) o [`SetStyle`](../setstyle/) per applicare la modifica a questa colonna. Lo stile della colonna è lo stile che verrà ereditato dalle celle in questa colonna (quelle celle che non hanno impostazioni di stile personalizzate, come le celle esistenti che non hanno avuto lo stile impostato esplicitamente, o quelle che non sono state istanziate)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodGetStyleDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta lo stile per la colonna 5
            Style columnStyle = cells.Columns[5].GetStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 14;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { Font = true });

            // Imposta lo stile per la riga 7
            Style rowStyle = cells.Rows[7].GetStyle();
            rowStyle.Font.Color = System.Drawing.Color.Red;
            rowStyle.Font.IsItalic = true;
            cells.Rows[7].ApplyStyle(rowStyle, new StyleFlag { Font = true });

            // Verifica lo stile della colonna
            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style:");
            Console.WriteLine($"Font: {retrievedColumnStyle.Font.Name}, Size: {retrievedColumnStyle.Font.Size}, Bold: {retrievedColumnStyle.Font.IsBold}");

            // Verifica lo stile della riga
            Style retrievedRowStyle = cells.Rows[7].GetStyle();
            Console.WriteLine("\nRow 7 Style:");
            Console.WriteLine($"Color: {retrievedRowStyle.Font.Color}, Italic: {retrievedRowStyle.Font.IsItalic}");

            // Salva la cartella di lavoro
            workbook.Save("ColumnMethodGetStyleDemo_output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


