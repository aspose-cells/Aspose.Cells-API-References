---
title: "Klasse PivotField"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.PivotField‑Klasse. Stellt ein Feld in einem PivotTable‑Bericht dar. Das PivotField‑Objekt ist Mitglied der PivotFields‑Sammlung.  HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen GridPivotField. Diese Klasse wird nach 6 Monaten ab August 2014 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben könnten."
type: docs
url: /de/net/aspose.cells.gridweb.data/pivotfield/
---
## PivotField class

Stellt ein Feld in einem PivotTable‑Bericht dar. Das PivotField‑Objekt ist Mitglied der [`PivotFields`](../pivotfields/)‑Sammlung.  HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen GridPivotField. Diese Klasse wird nach 6 Monaten ab August 2014 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben könnten.

```csharp
[Obsolete("This class is obsolete; use GridPivotField instead")]
public class PivotField
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Caption](../../aspose.cells.gridweb.data/pivotfield/caption/) { get; set; } | Der Beschriftungstext für das Pivot‑Feld wird im Bericht angezeigt. Standardmäßig wird der Name angezeigt. |
| [FieldItems](../../aspose.cells.gridweb.data/pivotfield/fielditems/) { get; } | Liest die Daten des angegebenen Feldes. |
| [Function](../../aspose.cells.gridweb.data/pivotfield/function/) { get; set; } | Stellt die Funktion dar, die verwendet wird, um das PivotTable‑Feld zusammenzufassen (nur Datenfelder). Die Standardfunktion ist Count. |
| [Name](../../aspose.cells.gridweb.data/pivotfield/name/) { get; } | Liest den Namen. |
| [Orientation](../../aspose.cells.gridweb.data/pivotfield/orientation/) { get; set; } | Stellt den Ort des Feldes im angegebenen PivotTable-Bericht dar. |
| [Position](../../aspose.cells.gridweb.data/pivotfield/position/) { get; set; } | Stellt die Position des Feldes (erste, zweite, dritte usw.) unter allen Feldern seiner Orientierung (Zeilen, Spalten, Seiten) dar. Sie sollten die Get‑Methode aufrufen, nachdem Pivottable.DataBind aufgerufen wurde. |
| [SortOrder](../../aspose.cells.gridweb.data/pivotfield/sortorder/) { get; set; } | Stellt die Reihenfolge dar, die zum Sortieren des angegebenen PivotTable-Feldes verwendet wird. |

### Beispiele

```csharp

 [C#]

 //Liefert PivotFields von PivotTable[0]
 PivotField field1 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field1"];
 PivotField field2 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field2"];
 PivotField field3 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field3"];
 PivotField field4 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field4"];

 //Setzt den Speicherort der PivotFields
 field1.Orientation = PivotFieldOrientation.RowField;
 field2.Orientation = PivotFieldOrientation.RowField;
 field3.Orientation = PivotFieldOrientation.ColumnField;
 field4.Orientation = PivotFieldOrientation.DataField;

 //Setzt die Funktion des Datenfelds
 field3.Function = PivotFieldFunction.Sum;

 //Ändert die Reihenfolge der Zeilenfelder
 field2.Position = 1; //Or field1.Position = 2;

 [VB]

 'Gets PivotFields of PivotTable[0]
 Dim field1 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field1")
 Dim field2 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field2")
 Dim field3 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field3")
 Dim field4 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field4")

 'Sets Location of PivotFields
 field1.Orientation = PivotFieldOrientation.RowField
 field2.Orientation = PivotFieldOrientation.RowField
 field3.Orientation = PivotFieldOrientation.ColumnField
 field4.Orientation = PivotFieldOrientation.DataField

 'Sets function of data field
 field3.Function = PivotFieldFunction.Sum
 'Changes row fields order
 field2.Position = 1 'Or field1.Position = 2;

```

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


