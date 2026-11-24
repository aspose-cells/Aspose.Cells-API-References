---
title: "Klasse ListObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Tables.ListObject-Klasse. Stellt eine Tabelle in einem Arbeitsblatt dar"
type: docs
url: /de/net/aspose.cells.tables/listobject/
---
## ListObject class

Stellt eine Tabelle in einem Arbeitsblatt dar.

```csharp
public class ListObject
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription/) { get; set; } | Liest und setzt die alternative Beschreibung. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext/) { get; set; } | Liest und setzt den alternativen Text. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter/) { get; } | Liest den Auto-Filter dieser Tabelle. |
| [Comment](../../aspose.cells.tables/listobject/comment/) { get; set; } | Liest und setzt den Kommentar der Tabelle. |
| [DataRange](../../aspose.cells.tables/listobject/datarange/) { get; } | Liest den Datenbereich der Tabelle. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype/) { get; } | Liest den Datentyp der Datenquelle der Tabelle. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname/) { get; set; } | Liest und setzt den Anzeigenamen der Tabelle. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn/) { get; } | Liest die Endspalte des Bereichs. |
| [EndRow](../../aspose.cells.tables/listobject/endrow/) { get; } | Liest die Endzeile des Bereichs. |
| [HasAutoFilter](../../aspose.cells.tables/listobject/hasautofilter/) { get; set; } | Gibt an, ob der Auto-Filter auf diese Tabelle angewendet wird. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns/) { get; } | Ermittelt die [`ListColumn`](../listcolumn/) Liste dieser Tabelle. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable/) { get; } | Ermittelt die verknüpfte QueryTable. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow/) { get; set; } | Ermittelt und setzt, ob diese Tabelle die Kopfzeile anzeigt. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes/) { get; set; } | Gibt an, ob Spaltenstreifenformatierung angewendet wird. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn/) { get; set; } | Gibt an, ob die erste Spalte in der Tabelle den angewendeten Stil hat. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn/) { get; set; } | Gibt an, ob die letzte Spalte in der Tabelle den angewendeten Stil hat. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes/) { get; set; } | Gibt an, ob Zeilenstreifenformatierung angewendet wird. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals/) { get; set; } | Ermittelt und setzt, ob diese TAble die Summenzeile anzeigt. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn/) { get; } | Ermittelt die Startspalte des Bereichs. |
| [StartRow](../../aspose.cells.tables/listobject/startrow/) { get; } | Ermittelt die Startzeile des Bereichs. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename/) { get; set; } | Ermittelt und setzt den Tabellenvorlagennamen. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype/) { get; set; } | Ermittelt und die integrierte Tabellenformatvorlage. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap/) { get; } | Ermittelt ein [`XmlMap`](./xmlmap/) das für diese Liste verwendet wird. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange/)() | Wendet die Tabellenformatvorlage auf den Bereich an. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange)() | Konvertiert die Tabelle in einen Bereich. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange_1)(TableToRangeOptions) | Konvertiert die Tabelle in einen Bereich. |
| [Filter](../../aspose.cells.tables/listobject/filter/)() | (**Obsolet.**) Filtert die Tabelle. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula)(int, int, string) | Setzt die Formel in die Zelle der Tabelle. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula_1)(int, int, string, bool) | Setzt die Formel in die Zelle der Tabelle. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue)(int, int, object) | Setzt den Wert in die Zelle. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue_1)(int, int, object, bool) | Setzt den Wert in die Zelle. |
| [RemoveAutoFilter](../../aspose.cells.tables/listobject/removeautofilter/)() | Entfernt den Autofilter, der auf diese Tabelle angewendet wird. |
| [Resize](../../aspose.cells.tables/listobject/resize/)(int, int, int, int, bool) | Ändert die Größe des Bereichs des Listobjekts. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname/)() | Aktualisiert alle Namen der Listenspalten in den Zellen der Tabelle. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fülle das Arbeitsblatt mit einigen Daten
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

            // Füge ein ListObject (Tabelle) zum Arbeitsblatt hinzu
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Setze einige Eigenschaften des ListObject
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
            table.DisplayName = "SampleTable";
            table.Comment = "This is a sample table.";
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.ShowTableStyleRowStripes = true;
            table.ShowTableStyleColumnStripes = true;
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Speichere die Arbeitsmappe
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


