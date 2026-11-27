---
title: "Gränssnitt LightCellsDataHandler"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LightCellsDataHandler‑gränssnitt. Representerar celldatahanterare för att läsa stora kalkylbladsfiler i lättviktläge."
type: docs
url: /sv/net/aspose.cells/lightcellsdatahandler/
---
## LightCellsDataHandler interface

Representerar celldatas hanterare för att läsa stora kalkylbladsfiler i lättviktsläge.

```csharp
public interface LightCellsDataHandler
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ProcessCell](../../aspose.cells/lightcellsdatahandler/processcell/)(Cell) | Påbörjar bearbetning av en cell. |
| [ProcessRow](../../aspose.cells/lightcellsdatahandler/processrow/)(Row) | Påbörjar bearbetning av en rad. |
| [StartCell](../../aspose.cells/lightcellsdatahandler/startcell/)(int) | Förbereder bearbetning av en cell. |
| [StartRow](../../aspose.cells/lightcellsdatahandler/startrow/)(int) | Förbereder bearbetning av en rad. |
| [StartSheet](../../aspose.cells/lightcellsdatahandler/startsheet/)(Worksheet) | Påbörjar bearbetning av ett kalkylblad. |

### Anmärkningar

När en arbetsbok läses i detta läge, kommer [`StartSheet`](./startsheet/) att kontrolleras när varje kalkylblad i arbetsboken läses. För ett blad, om [`StartSheet`](./startsheet/) returnerar true, kommer all data och egenskaper för rader/celler i detta blad att kontrolleras och behandlas av implementationen av detta gränssnitt. För varje rad kommer [`StartRow`](./startrow/) att anropas för att kontrollera om den behöver bearbetas. Om en rad behöver bearbetas läses dess egenskaper först och användaren kan komma åt dem via [`ProcessRow`](./processrow/). Om radens celler också behöver bearbetas, ska [`ProcessRow`](./processrow/) returnera true och sedan kommer [`StartCell`](./startcell/) att anropas för varje befintlig cell i raden för att kontrollera om en cell behöver bearbetas. Om en cell behöver bearbetas, kommer [`ProcessCell`](./processcell/) att anropas för att bearbeta cellen enligt implementationen av detta gränssnitt. Observera att användaren endast bör arbeta med värdena och egenskaperna för det aktuella Rad/Cell‑objektet som tillhandahålls av motsvarande metod. Eftersom celldata läses från mallfilen i strömmningsläge kan de flesta andra objekt återställas/uppdateras senare efter att celldata har lästs in. Så när användaren arbetar med andra objekt i denna implementation kan dessa operationer eventuellt inte påverka objekten som finns i arbetsboken. Eller ännu värre, dessa operationer kan orsaka inkonsekvent data i arbetsboken och sedan leda till oväntade problem eller undantag senare. Därför, för alla andra objekt såsom former, kolumnbredder och stilar, villkorsstyrd formatering, …etc., vänligen manipulera dem inte i några metoder i denna implementation. Hantera dem istället efter att arbetsboken har konstruerats.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerDemo : LightCellsDataHandler
    {
        public static void LightCellsDataHandlerExample()
        {
            // Skapa en arbetsbok och läs in den med LightCellsDataHandler
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av LightCellsDataHandlerDemo
            LightCellsDataHandlerDemo handler = new LightCellsDataHandlerDemo();

            // Ställ in LightCellsDataHandler för arbetsboken
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = handler;

            // Läs in arbetsboken med de angivna inläsningsalternativen
            workbook = new Workbook("LargeFile_original.xlsx", loadOptions);

            // Spara arbetsboken för att demonstrera processen
            workbook.Save("ProcessedLargeFile.xlsx");
        }

        // Implementera metoden StartSheet
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine("Starting to process sheet: " + sheet.Name);
            return true; // Continue processing
        }

        // Implementera metoden StartRow
        public bool StartRow(int rowIndex)
        {
            Console.WriteLine("Starting to process row: " + rowIndex);
            return true; // Continue processing
        }

        // Implementera metoden ProcessRow
        public bool ProcessRow(Row row)
        {
            Console.WriteLine("Processing row: " + row.Index);
            return true; // Continue processing
        }

        // Implementera metoden StartCell
        public bool StartCell(int columnIndex)
        {
            Console.WriteLine("Starting to process cell in column: " + columnIndex);
            return true; // Continue processing
        }

        // Implementera metoden ProcessCell
        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine("Processing cell: " + cell.Name + " with value: " + cell.StringValue);
            return true; // Continue processing
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


