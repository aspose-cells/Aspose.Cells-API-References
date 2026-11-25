---
title: "Column.HasCustomStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Column. Indica se questa colonna ha impostazioni di stile personalizzate diverse dallo stile predefinito ereditato dal workbook"
type: docs
url: /it/net/aspose.cells/column/hascustomstyle/
---
## Column.HasCustomStyle property

Indica se questa colonna ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dal workbook).

```csharp
public bool HasCustomStyle { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla prima colonna
            Column column = worksheet.Cells.Columns[0];

            // Visualizza il valore iniziale di HasCustomState
            Console.WriteLine("Initial HasCustomStyle: " + column.HasCustomStyle);

            // Modifica lo stile della colonna per dimostrare la modifica di HasCustomStyle
            Style columnStyle = column.GetStyle();
            columnStyle.BackgroundColor = Color.LightBlue;
            column.SetStyle(columnStyle);

            // Visualizza il valore aggiornato di HasCustomStyle
            Console.WriteLine("After style modification - HasCustomStyle: " + column.HasCustomStyle);

            // Crea un'altra colonna con lo stile predefinito per il confronto
            Column secondColumn = worksheet.Cells.Columns[1];
            Console.WriteLine("Second column HasCustomStyle: " + secondColumn.HasCustomStyle);

            // Salva la cartella di lavoro
            workbook.Save("ColumnHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


