---
title: "StyleFlag.FontName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. L'impostazione del nome del carattere verrà applicata"
type: docs
url: /it/net/aspose.cells/styleflag/fontname/
---
## StyleFlag.FontName property

L'impostazione del nome del carattere sarà applicata.

```csharp
public bool FontName { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea dati di esempio
            cells["A1"].PutValue("Product Name");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Laptop");
            cells["B2"].PutValue(999.99);
            cells["A3"].PutValue("Phone");
            cells["B3"].PutValue(699.99);

            // Crea stili con diversi nomi di carattere
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.Name = "Arial";
            headerStyle.Font.IsBold = true;
            headerStyle.Font.Size = 14;

            Style priceStyle = workbook.CreateStyle();
            priceStyle.Font.Name = "Courier New";
            priceStyle.Custom = "$#,##0.00";

            // Applica lo stile intestazione con StyleFlag
            Aspose.Cells.Range headerRange = cells.CreateRange(0, 0, 1, 2);
            StyleFlag headerFlag = new StyleFlag();
            headerFlag.FontName = true;
            headerFlag.FontBold = true;
            headerFlag.FontSize = true;
            headerRange.ApplyStyle(headerStyle, headerFlag);

            // Applica lo stile prezzo con StyleFlag concentrandosi su FontName
            Aspose.Cells.Range priceRange = cells.CreateRange(1, 1, 2, 1);
            StyleFlag priceFlag = new StyleFlag();
            priceFlag.FontName = true;
            priceFlag.NumberFormat = true;
            priceRange.ApplyStyle(priceStyle, priceFlag);

            // Adatta automaticamente le colonne per una migliore visibilità
            worksheet.AutoFitColumns();

            // Salva la cartella di lavoro
            workbook.Save("FontNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


