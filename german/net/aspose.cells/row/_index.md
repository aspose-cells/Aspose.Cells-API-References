---
title: Row
second_title: Aspose.Cells für .NET-API-Referenz
description: Stellt eine einzelne Zeile in einem Arbeitsblatt dar.
type: docs
weight: 5500
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
| [FirstCell](../../aspose.cells/row/firstcell) { get; } | Ruft das erste Zellobjekt in der Zeile ab. |
| [FirstDataCell](../../aspose.cells/row/firstdatacell) { get; } | Ruft die erste nicht leere Zelle in der Zeile ab. |
| [GroupLevel](../../aspose.cells/row/grouplevel) { get; } | Ruft die Gruppenebene der Zeile ab. |
| [Height](../../aspose.cells/row/height) { get; set; } | Holt und setzt die Zeilenhöhe in Punkteinheiten. |
| [Index](../../aspose.cells/row/index) { get; } | Ruft den Index dieser Zeile ab. |
| [IsBlank](../../aspose.cells/row/isblank) { get; } | Gibt an, ob die Zeile Daten enthält |
| [IsCollapsed](../../aspose.cells/row/iscollapsed) { get; set; } | ob die Zeile eingeklappt ist |
| [IsHeightMatched](../../aspose.cells/row/isheightmatched) { get; set; } | Gibt an, dass Zeilenhöhe und Standardschrifthöhe übereinstimmen. |
| [IsHidden](../../aspose.cells/row/ishidden) { get; set; } | Gibt an, ob die Zeile ausgeblendet ist. |
| [Item](../../aspose.cells/row/item) { get; } | Ruft die Zelle ab. |
| [LastCell](../../aspose.cells/row/lastcell) { get; } | Ruft das letzte Zellenobjekt in der Zeile ab. |
| [LastDataCell](../../aspose.cells/row/lastdatacell) { get; } | Ruft die letzte nicht leere Zelle in der Zeile ab. |
| [Style](../../aspose.cells/row/style) { get; } | Repräsentiert den Stil dieser Zeile. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ApplyStyle](../../aspose.cells/row/applystyle)(Style, StyleFlag) | Wendet Formate für eine ganze Zeile an. |
| [CopySettings](../../aspose.cells/row/copysettings)(Row, bool) | Kopieren Sie die Einstellungen der Zeile, wie Stil, Höhe, Sichtbarkeit usw. |
| [Equals](../../aspose.cells/row/equals#equals_1)(object) | Prüft, ob dieses Objekt mit einem anderen auf dieselbe Zeile verweist. |
| [Equals](../../aspose.cells/row/equals#equals)(Row) | Prüft, ob dieses Objekt auf dieselbe Zeile mit einem anderen Zeilenobjekt verweist. |
| [GetCellOrNull](../../aspose.cells/row/getcellornull)(int) | Ruft die Zelle oder Null im spezifischen Index ab. |
| [GetEnumerator](../../aspose.cells/row/getenumerator)() | Ruft die Zellen enumerator ab |

### Beispiele

```csharp

[C#]

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();

// Abrufen der Referenz des ersten Arbeitsblatts
Worksheet worksheet = workbook.Worksheets[0];
Style style = workbook.CreateStyle();

// Setzen Sie die Hintergrundfarbe auf Blau
style.BackgroundColor = Color.Blue;

//Vordergrundfarbe auf Rot setzen
style.ForegroundColor= Color.Red;

// Hintergrundmuster einstellen
style.Pattern = BackgroundType.DiagonalStripe;

//Flag für neuen Stil
StyleFlag styleFlag = new StyleFlag();

//Alle Stile festlegen
styleFlag.All = true;

 //Erste Zeile abrufen
Row row = worksheet.Cells.Rows[0];
 //Stil auf die erste Zeile anwenden
row.ApplyStyle(style, styleFlag);

//Speichern der Excel-Datei
workbook.Save("book1.xls");

[VB.NET]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()

'Abrufen der Referenz des ersten Arbeitsblatts
Dim worksheet As Worksheet = workbook.Worksheets(0)

Dim style As Style = workbook.CreateStyle()

'Setzen Sie die Hintergrundfarbe auf Blau
style.BackgroundColor = Color.Blue

'Setzen Sie die Vordergrundfarbe auf Rot
style.ForegroundColor = Color.Red

'Einstellung Hintergrundmuster
style.Pattern = BackgroundType.DiagonalStripe

'Flagge im neuen Stil
Dim styleFlag As New StyleFlag()

'Alle Stile einstellen
styleFlag.All = True

 'Erste Reihe erhalten
Dim row as Row = worksheet.Cells.Rows(0)
 'Wenden Sie Stil auf die erste Reihe an
row.ApplyStyle(style, styleFlag)

'Speichern der Excel-Datei
workbook.Save("book1.xls")
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
