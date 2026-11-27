---
title: "Klass ListObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Tables.ListObject class. Representerar en tabell i ett arbetsblad"
type: docs
url: /sv/net/aspose.cells.tables/listobject/
---
## ListObject class

Representerar en tabell i ett arbetsblad.

```csharp
public class ListObject
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription/) { get; set; } | Hämtar och anger den alternativa beskrivningen. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext/) { get; set; } | Hämtar och anger den alternativa texten. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter/) { get; } | Hämtar autofilter för den här tabellen. |
| [Comment](../../aspose.cells.tables/listobject/comment/) { get; set; } | Hämtar och anger kommentaren för tabellen. |
| [DataRange](../../aspose.cells.tables/listobject/datarange/) { get; } | Hämtar dataintervallet för tabellen. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype/) { get; } | Hämtar datakälltypen för tabellen. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname/) { get; set; } | Hämtar och anger visningsnamnet för tabellen. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn/) { get; } | Hämtar den sista kolumnen i intervallet. |
| [EndRow](../../aspose.cells.tables/listobject/endrow/) { get; } | Hämtar den sista raden i intervallet. |
| [HasAutoFilter](../../aspose.cells.tables/listobject/hasautofilter/) { get; set; } | Anger om autofilter är tillämpat på den här tabellen. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns/) { get; } | Hämtar [`ListColumn`](../listcolumn/) listan för den här tabellen. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable/) { get; } | Hämtar den länkade QueryTable. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow/) { get; set; } | Hämtar och anger om den här Table visar rubrikraden. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes/) { get; set; } | Anger om kolumnrandig formatering är tillämpad på. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn/) { get; set; } | Anger om den första kolumnen i tabellen är den stil som tillämpas på. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn/) { get; set; } | Anger om den sista kolumnen i tabellen är den stil som tillämpas på. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes/) { get; set; } | Anger om radrandig formatering är tillämpad på. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals/) { get; set; } | Hämtar och anger om den här TAble visar totalrad. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn/) { get; } | Hämtar startkolumnen i intervallet. |
| [StartRow](../../aspose.cells.tables/listobject/startrow/) { get; } | Hämtar startraden i intervallet. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename/) { get; set; } | Hämtar och anger tabellens stilnamn. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype/) { get; set; } | Hämtar och den inbyggda tabellstilen. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap/) { get; } | Hämtar en [`XmlMap`](./xmlmap/) som används för den här listan. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange/)() | Tillämpa tabellstilen på intervallet. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange)() | Konvertera tabellen till ett intervall. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange_1)(TableToRangeOptions) | Konvertera tabellen till ett intervall. |
| [Filter](../../aspose.cells.tables/listobject/filter/)() | (**Föråldrad.**) Filtrera tabellen. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula)(int, int, string) | Placera formeln i cellen i tabellen. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula_1)(int, int, string, bool) | Placera formeln i cellen i tabellen. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue)(int, int, object) | Placera värdet i cellen. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue_1)(int, int, object, bool) | Placera värdet i cellen. |
| [RemoveAutoFilter](../../aspose.cells.tables/listobject/removeautofilter/)() | Tar bort autofilter som är tillämpat på den här tabellen. |
| [Resize](../../aspose.cells.tables/listobject/resize/)(int, int, int, int, bool) | Ändra storlek på intervallet för listobjektet. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname/)() | Uppdaterar alla listkolumners namn till cellerna i tabellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectDemo
    {
        public static void ListObjectExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i arbetsbladet med några data
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Lägg till ett ListObject (tabell) i kalkylbladet
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Ställ in vissa egenskaper för ListObject
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
            table.DisplayName = "SampleTable";
            table.Comment = "This is a sample table.";
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.ShowTableStyleRowStripes = true;
            table.ShowTableStyleColumnStripes = true;
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Spara arbetsboken
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


