---
title: "Style.Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore Style. Inizializza una nuova istanza della classe Style"
type: docs
url: /it/net/aspose.cells/style/style/
---
## Style constructor

Inizializza una nuova istanza della classe [`Style`](../).

```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```

### Osservazioni

NOTA: Questo costruttore è ora obsoleto. Invece, si prega di utilizzare il metodo CellsFactory.CreateStyle(). Questa proprietà sarà rimossa 6 mesi dopo da ottobre 2016. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile utilizzando il costruttore
            Style style = new Style();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;

            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Text");
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("StyleConstructorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


