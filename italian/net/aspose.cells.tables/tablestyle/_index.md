---
title: "Classe TableStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Tables.TableStyle. Rappresenta lo stile della tabella"
type: docs
url: /it/net/aspose.cells.tables/tablestyle/
---
## TableStyle class

Rappresenta lo stile della tabella.

```csharp
public class TableStyle
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Name](../../aspose.cells.tables/tablestyle/name/) { get; } | Ottiene il nome dello stile della tabella. |
| [TableStyleElements](../../aspose.cells.tables/tablestyle/tablestyleelements/) { get; } | Ottiene tutti gli elementi dello stile della tabella. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Create](../../aspose.cells.tables/tablestyle/create/)(string, WorksheetCollection) | Crea uno stile vuoto per tabella/tabella pivot. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleDemo
    {
        public static void TableStyleExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea stili per la prima e l'ultima colonna
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Definisci un nome di stile di tabella personalizzato
            string tableStyleName = "Custom1";

            // Accedi alla raccolta degli stili di tabella
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Aggiungi un nuovo stile di tabella alla raccolta
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Accedi alla raccolta degli elementi dello stile di tabella
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Aggiungi e imposta lo stile per la prima colonna
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Aggiungi e imposta lo stile per l'ultima colonna
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Accedi alle celle del primo foglio di lavoro
            Cells cells = workbook.Worksheets[0].Cells;

            // Popola la prima riga con i nomi delle colonne
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }

            // Popola il resto delle celle con dati di esempio
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Aggiungi una tabella al foglio di lavoro
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Applica lo stile di tabella personalizzato alla tabella
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Salva la cartella di lavoro
            workbook.Save("TableStyleExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


