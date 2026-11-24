---
title: "Klasse Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Name class. Stellt einen definierten Namen für einen Zellbereich dar."
type: docs
url: /de/net/aspose.cells/name/
---
## Name class

Stellt einen definierten Namen für einen Zellbereich dar.

```csharp
public class Name
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Comment](../../aspose.cells/name/comment/) { get; set; } | Liest und setzt den Kommentar des Namens. Gilt nur für Excel 2007 oder neuere Versionen. |
| [FullText](../../aspose.cells/name/fulltext/) { get; } | Liest den vollständigen Text des Namens des Objekts mit der Geltungsbereichseinstellung. |
| [IsReferred](../../aspose.cells/name/isreferred/) { get; } | Gibt an, ob dieser Name von anderen Formeln referenziert wird. |
| [IsVisible](../../aspose.cells/name/isvisible/) { get; set; } | Gibt an, ob der Name sichtbar ist. |
| [R1C1RefersTo](../../aspose.cells/name/r1c1refersto/) { get; set; } | Liest oder setzt eine R1C1-Referenz des `Name`. |
| [RefersTo](../../aspose.cells/name/refersto/) { get; set; } | Liest oder setzt die Formel, auf die der Name definiert ist, beginnend mit einem Gleichheitszeichen. |
| [SheetIndex](../../aspose.cells/name/sheetindex/) { get; set; } | Gibt an, ob dieser Name zu einer Arbeitsmappe oder einem Arbeitsblatt gehört. 0 = Globaler Name, sonst Index zum Blatt (einsbasiert). |
| [Text](../../aspose.cells/name/text/) { get; set; } | Liest den Namens-Text des Objekts. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetRange](../../aspose.cells/name/getrange/#getrange)() | Liest den Bereich, wenn sich dieser Name auf einen Bereich bezieht. |
| [GetRange](../../aspose.cells/name/getrange/#getrange_1)(bool) | Liest den Bereich, wenn sich dieser Name auf einen Bereich bezieht |
| [GetRange](../../aspose.cells/name/getrange/#getrange_2)(int, int, int) | Liest den Bereich, wenn sich dieser Name auf einen Bereich bezieht. Wenn die Referenz dieses Namens nicht absolut ist, kann der Bereich für verschiedene Zellen unterschiedlich sein. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges)() | Liest alle Bereiche, auf die dieser Name verweist. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges_1)(bool) | Liest alle Bereiche, auf die dieser Name verweist. |
| [GetReferredAreas](../../aspose.cells/name/getreferredareas/)(bool) | Liest alle Referenzen, auf die dieser Name verweist. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto)(bool, bool) | Lese die Referenz dieses Namens. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto_1)(bool, bool, int, int) | Lese die Referenz dieses Namens basierend auf der angegebenen Zelle. |
| [SetRefersTo](../../aspose.cells/name/setrefersto/)(string, bool, bool) | Setze die Referenz dieses Namens. |
| override [ToString](../../aspose.cells/name/tostring/)() | Gibt einen String zurück, der das aktuelle Range-Objekt darstellt. |

### Beispiele

```csharp

[C#]

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();
//Zugriff auf das erste Arbeitsblatt in der Excel-Datei
Worksheet worksheet = workbook.Worksheets[0];
//Erstellen eines benannten Bereichs
Range range = worksheet.Cells.CreateRange("B4", "G14");
//Festlegen des Namens des benannten Bereichs
range.Name = "TestRange";
//Speichern der modifizierten Excel-Datei im Standardformat (das ist Excel 2000)
workbook.Save("output.xls");   

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Accessing the first worksheet in the Excel file
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Creating a named range
Dim range As Range = worksheet.Cells.CreateRange("B4", "G14")
'Setting the name of the named range
range.Name = "TestRange"
'Saving the modified Excel file in default (that is Excel 2000) format
workbook.Save("output.xls")
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


