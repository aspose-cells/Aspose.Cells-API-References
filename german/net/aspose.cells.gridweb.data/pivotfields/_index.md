---
title: "Klasse PivotFields"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.PivotFields Klasse. Stellt eine Sammlung aller PivotField‑Objekte in einem PivotTable‑Bericht dar"
type: docs
url: /de/net/aspose.cells.gridweb.data/pivotfields/
---
## PivotFields class

Stellt eine Sammlung aller [`PivotField`](../pivotfield/) Objekte in einem PivotTable‑Bericht dar.

```csharp
[Obsolete("This class is obsolete; use GridPivotFieldCollection instead")]
public class PivotFields : ICollection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotfields/count/) { get; } | Liest die Anzahl der im PivotFields‑Instanz enthaltenen Elemente |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotfields/issynchronized/) { get; } | Liest einen Wert, der angibt, ob der Zugriff auf die PivotFields synchronisiert (thread‑sicher) ist. |
| [Item](../../aspose.cells.gridweb.data/pivotfields/item/) { get; } | Liest ein PivotField nach Index. (2 Indexer) |
| [Parent](../../aspose.cells.gridweb.data/pivotfields/parent/) { get; } | Liefert das übergeordnete Objekt für das angegebene Objekt. Nur lesbar. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotfields/syncroot/) { get; } | Liest ein Objekt, das zum Synchronisieren des Zugriffs auf die PivotFields verwendet werden kann. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CopyTo](../../aspose.cells.gridweb.data/pivotfields/copyto/)(Array, int) | Kopiert das gesamte PivotField in ein kompatibles eindimensionales Array, beginnend am angegebenen Index des Zielarrays |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotfields/getenumerator/)() | Gibt einen IEnumerator für die PivotFields zurück. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotfields/indexof/)(PivotField) | Liest den Index des angegebenen PivotField. |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen GridPivotFieldCollection. Diese Klasse wird nach 6 Monaten ab August 2014 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

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


