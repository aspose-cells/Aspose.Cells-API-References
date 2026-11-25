---
title: "StyleFlag.DiagonalDownBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verranno applicate le impostazioni del bordo diagonale verso il basso"
type: docs
url: /it/net/aspose.cells/styleflag/diagonaldownborder/
---
## StyleFlag.DiagonalDownBorder property

Le impostazioni del bordo diagonale verso il basso saranno applicate.

```csharp
public bool DiagonalDownBorder { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalDownBorderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta del testo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Down Border Demo");

            // Crea un oggetto stile e imposta il bordo diagonale verso il basso
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 0, 255);
            
            // Crea un flag di stile e abilita il flag del bordo diagonale verso il basso
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalDownBorder = true;

            // Applica lo stile con il flag alla cella
            cell.SetStyle(style, styleFlag);

            // Verifica se il flag del bordo diagonale verso il basso è abilitato
            Console.WriteLine("DiagonalDownBorder flag is enabled: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);

            // Disabilita il flag del bordo diagonale verso il basso
            styleFlag.DiagonalDownBorder = false;
            style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 255, 0);

            // Applica lo stile con il flag alla cella
            cell.SetStyle(style, styleFlag);
            Console.WriteLine("DiagonalDownBorder flag is now: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);

            // Salva la cartella di lavoro
            workbook.Save("StyleFlagPropertyDiagonalDownBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


