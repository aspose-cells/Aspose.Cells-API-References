---
title: "TableStyleElement.Size"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TableStyleElement. Numero di righe o colonne in una singola banda di strisce. Si applica solo quando il tipo è firstRowStripe secondRowStripe firstColumnStripe o secondColumnStripe"
type: docs
url: /it/net/aspose.cells.tables/tablestyleelement/size/
---
## TableStyleElement.Size property

Numero di righe o colonne in una singola banda di strisce. Si applica solo quando il tipo è firstRowStripe, secondRowStripe, firstColumnStripe o secondColumnStripe.

```csharp
public int Size { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertySizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare una tabella
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Crea una tabella
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Crea uno stile di tabella usando la collezione di stili della cartella di lavoro
            TableStyleCollection styleCollection = workbook.Worksheets.TableStyles;
            int styleIndex = styleCollection.AddTableStyle("CustomStyle");
            TableStyle style = styleCollection[styleIndex];
            table.TableStyleName = style.Name;

            // Aggiungi elementi a strisce per dimostrare la proprietà Size
            style.TableStyleElements.Add(TableStyleElementType.FirstRowStripe);
            style.TableStyleElements.Add(TableStyleElementType.SecondRowStripe);

            // Accedi agli elementi a strisce
            TableStyleElement firstStripe = style.TableStyleElements[TableStyleElementType.FirstRowStripe];
            TableStyleElement secondStripe = style.TableStyleElements[TableStyleElementType.SecondRowStripe];

            // Visualizza i valori attuali di Size
            Console.WriteLine("Initial First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Initial Second Stripe Size: " + secondStripe.Size);

            // Modifica le dimensioni delle strisce
            firstStripe.Size = 2;
            secondStripe.Size = 3;

            // Visualizza i valori modificati
            Console.WriteLine("Modified First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Modified Second Stripe Size: " + secondStripe.Size);

            // Salva la cartella di lavoro per vedere gli effetti
            workbook.Save("TableStyleElementSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


