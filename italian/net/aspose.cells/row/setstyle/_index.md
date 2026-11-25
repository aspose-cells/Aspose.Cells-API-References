---
title: "Row.SetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Row. Imposta lo stile di questa riga"
type: docs
url: /it/net/aspose.cells/row/setstyle/
---
## Row.SetStyle method

Imposta lo stile di questa riga.

```csharp
public void SetStyle(Style style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | lo stile da utilizzare come stile predefinito per le celle in questa riga. |

### Osservazioni

Questo metodo imposta solo lo stile fornito come stile predefinito per questa riga, senza modificare le impostazioni di stile delle celle esistenti in questa riga. Per aggiornare le impostazioni di stile delle celle esistenti allo stile specificato contemporaneamente, si prega di utilizzare [`ApplyStyle`](../applystyle/)

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea e configura uno stile
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Blue;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.DiagonalStripe;

            // Ottieni la prima riga e applica lo stile
            Row row = worksheet.Cells.Rows[0];
            row.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("RowStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


