---
title: "Klass TableStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Tables.TableStyle-klass. Representerar stil för tabellen"
type: docs
url: /sv/net/aspose.cells.tables/tablestyle/
---
## TableStyle class

Representerar tabellens stil.

```csharp
public class TableStyle
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Name](../../aspose.cells.tables/tablestyle/name/) { get; } | Hämtar namnet på tabellstil. |
| [TableStyleElements](../../aspose.cells.tables/tablestyle/tablestyleelements/) { get; } | Hämtar alla element i tabellstilen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [Create](../../aspose.cells.tables/tablestyle/create/)(string, WorksheetCollection) | Skapar en tom tabell-/pivottabellstil. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa stilar för den första och sista kolumnen
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Definiera ett anpassat tabellstilsnamn
            string tableStyleName = "Custom1";

            // Få åtkomst till samlingen av tabellstilar
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Lägg till en ny tabellstil i samlingen
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Få åtkomst till samlingen av tabellstilelement
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Lägg till och ange stil för den första kolumnen
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Lägg till och ange stil för den sista kolumnen
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Åtkomst till cellerna i det första kalkylbladet
            Cells cells = workbook.Worksheets[0].Cells;

            // Fyll den första raden med kolumnnamn
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }

            // Fyll resten av cellerna med exempeldata
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Lägg till en tabell i kalkylbladet
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Tillämpa den anpassade tabellstilen på tabellen
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Spara arbetsboken
            workbook.Save("TableStyleExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


