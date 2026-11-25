---
title: "CellsHelper.GetUsedColors"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Ottiene tutti i colori usati nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells/cellshelper/getusedcolors/
---
## CellsHelper.GetUsedColors method

Ottiene tutti i colori utilizzati nella cartella di lavoro.

```csharp
public static Color[] GetUsedColors(Workbook workbook)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cartella di lavoro | Cartella di lavoro | L'oggetto cartella di lavoro. |

### Valore di ritorno

I colori usati.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsHelperMethodGetUsedColorsWithWorkbookDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcune celle colorate per dimostrare i colori usati
            worksheet.Cells["A1"].PutValue("Red Cell");
            worksheet.Cells["A1"].GetStyle().ForegroundColor = Color.Red;
            worksheet.Cells["A1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["A1"].SetStyle(worksheet.Cells["A1"].GetStyle());

            worksheet.Cells["B1"].PutValue("Blue Cell");
            worksheet.Cells["B1"].GetStyle().ForegroundColor = Color.Blue;
            worksheet.Cells["B1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["B1"].SetStyle(worksheet.Cells["B1"].GetStyle());

            worksheet.Cells["C1"].PutValue("Green Cell");
            worksheet.Cells["C1"].GetStyle().ForegroundColor = Color.Green;
            worksheet.Cells["C1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["C1"].SetStyle(worksheet.Cells["C1"].GetStyle());

            try
            {
                // Chiama il metodo GetUsedColors con il parametro cartella di lavoro
                Color[] usedColors = CellsHelper.GetUsedColors(workbook);

                // Visualizza i colori usati
                Console.WriteLine("Used colors in the workbook:");
                foreach (Color color in usedColors)
                {
                    Console.WriteLine($"Color: A={color.A}, R={color.R}, G={color.G}, B={color.B}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetUsedColors method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CellsHelperGetUsedColorsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../../workbook/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


