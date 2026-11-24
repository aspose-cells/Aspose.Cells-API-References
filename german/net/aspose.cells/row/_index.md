---
title: "Klasse Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Row Klasse. Stellt eine einzelne Zeile in einem Arbeitsblatt dar"
type: docs
url: /de/net/aspose.cells/row/
---
## Row class

Stellt eine einzelne Zeile in einem Arbeitsblatt dar.

```csharp
public class Row : IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FirstCell](../../aspose.cells/row/firstcell/) { get; } | Gibt das erste Zellenobjekt in der Zeile zurück. |
| [FirstDataCell](../../aspose.cells/row/firstdatacell/) { get; } | Gibt die erste nicht leere Zelle in der Zeile zurück. |
| [GroupLevel](../../aspose.cells/row/grouplevel/) { get; set; } | Gibt die Gruppierungsebene der Zeile zurück. |
| [HasCustomStyle](../../aspose.cells/row/hascustomstyle/) { get; } | Gibt an, ob diese Zeile benutzerdefinierte Stileinstellungen hat (anders als die standardmäßige, die vom Arbeitsbuch geerbt wird). |
| [Height](../../aspose.cells/row/height/) { get; set; } | Liest und setzt die Zeilenhöhe in Punkten. |
| [Index](../../aspose.cells/row/index/) { get; } | Gibt den Index dieser Zeile zurück. |
| [IsBlank](../../aspose.cells/row/isblank/) { get; } | Gibt an, ob die Zeile Daten enthält |
| [IsCollapsed](../../aspose.cells/row/iscollapsed/) { get; set; } | ob die Zeile zusammengeklappt ist |
| [IsHeightMatched](../../aspose.cells/row/isheightmatched/) { get; set; } | Gibt an, ob die Zeilenhöhe mit der aktuellen Standardschriftart-Einstellung des Arbeitsbuchs übereinstimmt. Der Wert true dieser Eigenschaft bedeutet außerdem, dass die Zeilenhöhe "automatisch" ist, ohne dass ein benutzerdefinierter Höhenwert vom Benutzer festgelegt wurde. |
| [IsHidden](../../aspose.cells/row/ishidden/) { get; set; } | Gibt an, ob die Zeile ausgeblendet ist. |
| [Item](../../aspose.cells/row/item/) { get; } | Gibt die Zelle zurück. |
| [LastCell](../../aspose.cells/row/lastcell/) { get; } | Gibt das letzte Zellenobjekt in der Zeile zurück. |
| [LastDataCell](../../aspose.cells/row/lastdatacell/) { get; } | Gibt die letzte nicht leere Zelle in der Zeile zurück. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ApplyStyle](../../aspose.cells/row/applystyle/)(Style, StyleFlag) | Wendet Formate für eine ganze Zeile an. |
| [CopySettings](../../aspose.cells/row/copysettings/)(Row, bool) | Kopiert Einstellungen der Zeile, wie Stil, Höhe, Sichtbarkeit, ...usw. |
| override [Equals](../../aspose.cells/row/equals/#equals_1)(object) | Überprüft, ob dieses Objekt auf dieselbe Zeile wie ein anderes verweist. |
| [Equals](../../aspose.cells/row/equals/#equals)(Row) | Überprüft, ob dieses Objekt auf dieselbe Zeile wie ein anderes Zeilenobjekt verweist. |
| [GetCellByIndex](../../aspose.cells/row/getcellbyindex/)(int) | Ruft die Zelle anhand eines bestimmten Indexes in der Zellsammlung dieser Zeile ab. |
| [GetCellOrNull](../../aspose.cells/row/getcellornull/)(int) | Gibt die Zelle oder null am angegebenen Index zurück. |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator)() | Gibt den Zellen-Enumerator zurück |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator_1)(bool, bool) | Gibt einen Enumerator zurück, der die Zellen dieser Zeile durchläuft. |
| [GetStyle](../../aspose.cells/row/getstyle/)() | Gibt den Stil dieser Zeile zurück. |
| [SetStyle](../../aspose.cells/row/setstyle/)(Style) | Setzt den Stil dieser Zeile. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;
    using System.Collections;

    public class RowDemo
    {
        public static void RowExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Ermitteln der Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie ein Stilobjekt
            Style style = workbook.CreateStyle();

            // Setzt die Hintergrundfarbe auf Blau
            style.BackgroundColor = Color.Blue;

            // Setzt die Vordergrundfarbe auf Rot
            style.ForegroundColor = Color.Red;

            // Setzt das Hintergrundmuster
            style.Pattern = BackgroundType.DiagonalStripe;

            // Neues Stil-Flag
            StyleFlag styleFlag = new StyleFlag();

            // Alle Stile festlegen
            styleFlag.All = true;

            // Erste Zeile abrufen
            Row row = worksheet.Cells.Rows[0];

            // Stil auf die erste Zeile anwenden
            row.ApplyStyle(style, styleFlag);

            // Zeilen-Eigenschaften festlegen
            row.Height = 20.0;
            row.IsHidden = false;
            row.IsCollapsed = false;
            row.GroupLevel = 1;
            row.IsHeightMatched = true;

            // Zugriff auf Zellen in der Zeile
            Cell firstCell = row.FirstCell;
            Cell firstDataCell = row.FirstDataCell;
            Cell lastCell = row.LastCell;
            Cell lastDataCell = row.LastDataCell;

            // Überprüfen, ob die Zeile leer ist
            bool isBlank = row.IsBlank;

            // Überprüfen, ob die Zeile einen benutzerdefinierten Stil hat
            bool hasCustomStyle = row.HasCustomStyle;

            // Abrufen des Index der Zeile
            int rowIndex = row.Index;

            // Abrufen einer Zelle nach Index
            Cell cellByIndex = row.GetCellByIndex(0);

            // Abrufen des Stils der Zeile
            Style rowStyle = row.GetStyle();

            // Festlegen des Stils der Zeile
            row.SetStyle(rowStyle);

            // Einstellungen von einer anderen Zeile kopieren
            Row sourceRow = worksheet.Cells.Rows[1];
            row.CopySettings(sourceRow, true);

            // Durch die Zellen in der Zeile iterieren
            IEnumerator cellEnumerator = row.GetEnumerator();
            while (cellEnumerator.MoveNext())
            {
                Cell cell = (Cell)cellEnumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Die Excel-Datei speichern
            workbook.Save("RowExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


