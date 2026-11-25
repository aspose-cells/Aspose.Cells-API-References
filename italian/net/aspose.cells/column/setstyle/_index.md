---
title: "Column.SetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Column. Imposta lo stile di questa colonna"
type: docs
url: /it/net/aspose.cells/column/setstyle/
---
## Column.SetStyle method

Imposta lo stile di questa colonna.

```csharp
public void SetStyle(Style style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | lo stile da utilizzare come stile predefinito per le celle in questa colonna. |

### Osservazioni

Questo metodo imposta solo lo stile fornito come stile predefinito per questa colonna, senza modificare le impostazioni di stile delle celle esistenti in questa colonna. Per aggiornare le impostazioni di stile delle celle esistenti allo stile specificato contemporaneamente, si prega di utilizzare [`ApplyStyle`](../applystyle/)

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnMethodSetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla prima colonna
            Column column = worksheet.Cells.Columns[0];

            // Crea un nuovo stile dal workbook
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            try
            {
                // Applica lo stile personalizzato all'intera colonna
                column.SetStyle(style);
                
                Console.WriteLine($"Style applied successfully to column {column.Index}");
                Console.WriteLine($"Font: {style.Font.Name}, Size: {style.Font.Size}, Bold: {style.Font.IsBold}");
                Console.WriteLine($"Background: {style.ForegroundColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("ColumnMethodSetStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


