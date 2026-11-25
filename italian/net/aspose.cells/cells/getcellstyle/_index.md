---
title: "Cells.GetCellStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottieni lo stile della cella specificata"
type: docs
url: /it/net/aspose.cells/cells/getcellstyle/
---
## Cells.GetCellStyle method

Ottieni lo stile della cella fornita.

```csharp
public Style GetCellStyle(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | indice della riga |
| colonna | Int32 | colonna |

### Valore di ritorno

lo stile della cella specificata.

### Osservazioni

Lo stile restituito è solo quello impostato per la cella o ereditato dalla riga/colonna della cella, non include le proprietà applicate da altre impostazioni come la formattazione condizionale.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsMethodGetCellStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella B5 (riga 4, colonna 1) e imposta lo stile iniziale
            Cell cell = worksheet.Cells["B5"];
            cell.PutValue("Styled Cell");
            
            // Crea e applica lo stile iniziale della cella
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.IsBold = true;  // Changed from Bold to IsBold
            initialStyle.BackgroundColor = Color.LightYellow;
            cell.SetStyle(initialStyle);

            try
            {
                // Chiama GetCellStyle con parametri Int32 (riga 4, colonna 1)
                Style cellStyle = worksheet.Cells.GetCellStyle(4, 1);

                // Visualizza le proprietà dello stile recuperato
                Console.WriteLine($"Retrieved style - Bold: {cellStyle.Font.IsBold}, Background: {cellStyle.BackgroundColor}");  // Changed from Bold to IsBold

                // Modifica lo stile recuperato
                cellStyle.Font.IsItalic = true;  // Changed from Italic to IsItalic
                cellStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

                // Applica lo stile modificato nuovamente alla cella
                cell.SetStyle(cellStyle);

                Console.WriteLine("GetCellStyle executed successfully. Modified border and font style.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellStyle: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("CellsGetCellStyleWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


