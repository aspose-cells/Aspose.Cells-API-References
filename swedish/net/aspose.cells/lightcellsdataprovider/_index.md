---
title: "Gränssnitt LightCellsDataProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LightCellsDataProvider‑gränssnitt. Representerar dataleverantör för att spara stora kalkylbladsfiler i lättviktsläge."
type: docs
url: /sv/net/aspose.cells/lightcellsdataprovider/
---
## LightCellsDataProvider interface

Representerar dataleverantör för att spara stora kalkylbladsfiler i lättviktsläge.

```csharp
public interface LightCellsDataProvider
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [IsGatherString](../../aspose.cells/lightcellsdataprovider/isgatherstring/)() | Kontrollerar om det aktuella strängvärdet i cellen behöver samlas in i en global pool. |
| [NextCell](../../aspose.cells/lightcellsdataprovider/nextcell/)() | Hämtar nästa cell som ska sparas. |
| [NextRow](../../aspose.cells/lightcellsdataprovider/nextrow/)() | Hämtar nästa rad som ska sparas. |
| [StartCell](../../aspose.cells/lightcellsdataprovider/startcell/)(Cell) | Påbörjar sparandet av data för en cell. |
| [StartRow](../../aspose.cells/lightcellsdataprovider/startrow/)(Row) | Påbörjar sparandet av data för en rad. |
| [StartSheet](../../aspose.cells/lightcellsdataprovider/startsheet/)(int) | Påbörjar sparandet av ett kalkylblad. |

### Anmärkningar

När en arbetsbok sparas med detta läge kommer [`StartSheet`](./startsheet/) att kontrolleras vid sparning av varje kalkylblad i arbetsboken. För ett blad, om [`StartSheet`](./startsheet/) returnerar true, kommer all data och egenskaper som ska sparas för rader/celler i detta blad att tillhandahållas av implementeringen av detta gränssnitt. Först kommer [`NextRow`](./nextrow/) att anropas för att få nästa radindex som ska sparas. Om ett giltigt radindex returneras (radindexet måste vara i stigande ordning för de rader som ska sparas), kommer ett Row‑objekt som representerar denna rad att tillhandahållas av [`StartRow`](./startrow/) så att implementeringen kan sätta dess egenskaper. För en rad kommer [`NextCell`](./nextcell/) att kontrolleras först. Om ett giltigt kolumnindex returneras (kolumnindexet måste vara i stigande ordning för alla celler i den aktuella raden), kommer ett Cell‑objekt som representerar denna cell att tillhandahållas av [`StartCell`](./startcell/) för att implementeringen ska kunna sätta dess data och egenskaper. Efter [`StartCell`](./startcell/) sparas cellen direkt till den resulterande kalkylbladsfilen. Därefter kontrolleras och bearbetas nästa cell.  Observera att användaren endast bör uppdatera värden och egenskaper för det aktuella Row/Cell‑objekt som tillhandahålls av motsvarande metod. Eftersom cellernas data skrivs till den resulterande filen i ett strömningssätt, kan de flesta andra objekt redan ha skrivits till filen eller ha samlats och skrivit någon global data för dem. Så när användaren uppdaterar andra objekt medan celldata sparas, kan dessa operationer eventuellt inte påverka den sparade datan. Ännu värre kan dessa operationer leda till inkonsekvent data som sparas till den resulterande filen och slutligen göra filen korrupt. Därför, för alla andra objekt såsom former, kolumnbredder och stilar, villkorsformatering, …etc., vänligen manipulera dem inte i någon metod i denna implementation. Hantera dem istället och justera dem till slutligt tillstånd innan du anropar metoden "Save" för arbetsboken.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderDemo
    {
        public static void LightCellsDataProviderExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en anpassad LightCellsDataProvider
            CustomLightCellsDataProvider dataProvider = new CustomLightCellsDataProvider();

            // Ställ in LightCellsDataProvider för att spara arbetsboken
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
            {
                LightCellsDataProvider = dataProvider
            };

            // Spara arbetsboken med den anpassade LightCellsDataProvider
            workbook.Save("LightCellsDataProviderExample.xlsx", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Starta bearbetning av det första bladet
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            // Gå till nästa rad
            currentRow++;
            currentCell = -1;

            // Returnera det aktuella radindexet eller -1 om det inte finns fler rader
            return currentRow < 10 ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Initiera raden om det behövs
        }

        public int NextCell()
        {
            // Gå till nästa cell
            currentCell++;

            // Returnera det aktuella cellindexet eller -1 om det inte finns fler celler
            return currentCell < 10 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            // Ange värdet för cellen
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            // Returnera om strängar ska samlas in i en global pool
            return false;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


