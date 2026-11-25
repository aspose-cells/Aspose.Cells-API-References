---
title: "Column.Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Column. Ottiene lo stile di questa colonna"
type: docs
url: /it/net/aspose.cells/column/style/
---
## Column.Style property

Restituisce lo stile di questa colonna.

```csharp
[Obsolete("Use Column.GetStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style Style { get; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Column.GetStyle() per ottenere lo stile predefinito di questa colonna. Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima colonna
            Column column = worksheet.Cells.Columns[0];
            
            // Ottieni lo stile corrente usando la proprietà Style
            Style originalStyle = column.Style;
            Console.WriteLine("Original column style - Background: " + originalStyle.BackgroundColor);
            
            // Crea un nuovo stile e modifica le proprietà
            Style newStyle = workbook.CreateStyle();
            newStyle.BackgroundColor = Color.LightBlue;
            newStyle.Font.IsBold = true;
            newStyle.HorizontalAlignment = TextAlignmentType.Center;
            
            // Applica il nuovo stile alla colonna
            column.SetStyle(newStyle);
            
            // Aggiungi dati per dimostrare l'applicazione dello stile
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Verifica le modifiche allo stile
            Console.WriteLine("New column style applied - Background: " + column.GetStyle().BackgroundColor);
            
            // Salva con regolazione della larghezza della colonna
            column.Width = 15;
            workbook.Save("ColumnStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


