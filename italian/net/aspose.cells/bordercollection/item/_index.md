---
title: "BorderCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BorderCollection. Ottiene l'elemento Border all'indice specificato"
type: docs
url: /it/net/aspose.cells/bordercollection/item/
---
## BorderCollection indexer

Ottiene l'elemento [`Border`](../../border/) all'indice specificato.

```csharp
public Border this[BorderType borderType] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| borderType | Il bordo da recuperare. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class BorderCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Ottieni la cella e il suo stile
                Cell cell = worksheet.Cells["A1"];
                Style style = cell.GetStyle();

                // Accedi a BorderCollection dallo stile
                BorderCollection borders = style.Borders;

                // Visualizza il valore corrente della proprietà Item (operazione di lettura)
                // Nota: la proprietà Item è di sola lettura e restituisce un oggetto Border
                // La proprietà Item richiede un parametro BorderType
                Border border = borders[BorderType.LeftBorder];
                Console.WriteLine("Border type: " + border.LineStyle);
                Console.WriteLine("Border color: " + border.Color);

                // Salva il risultato
                workbook.Save("ItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Border](../../border/)
* enum [BorderType](../../bordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


