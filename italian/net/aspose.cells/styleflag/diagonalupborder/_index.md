---
title: "StyleFlag.DiagonalUpBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Le impostazioni del bordo diagonale verso l'alto verranno applicate"
type: docs
url: /it/net/aspose.cells/styleflag/diagonalupborder/
---
## StyleFlag.DiagonalUpBorder property

Le impostazioni del bordo diagonale verso l'alto saranno applicate.

```csharp
public bool DiagonalUpBorder { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalUpBorderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta del testo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Crea un oggetto stile e imposta il bordo diagonale verso l'alto
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 0, 255);

            // Crea un flag di stile e abilita il flag del bordo diagonale verso l'alto
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalUpBorder = true;

            // Applica lo stile con il flag alla cella
            cell.SetStyle(style, styleFlag);

            // Crea un'altra cella per dimostrare l'effetto
            Cell cell2 = worksheet.Cells["B2"];
            cell2.PutValue("Diagonal Up Border Demo");

            // Crea uno stile diverso per il confronto
            Style style2 = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 255, 0);

            // Applica il secondo stile con lo stesso flag
            cell2.SetStyle(style2, styleFlag);

            // Salva la cartella di lavoro
            workbook.Save("StyleFlagPropertyDiagonalUpBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


