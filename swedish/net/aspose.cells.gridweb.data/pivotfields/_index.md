---
title: "Klass PivotFields"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.PivotFields-klass. Representerar en samling av alla PivotField-objekt i en PivotTable-rapport."
type: docs
url: /sv/net/aspose.cells.gridweb.data/pivotfields/
---
## PivotFields class

Representerar en samling av alla [`PivotField`](../pivotfield/) objekt i en PivotTable-rapport.

```csharp
[Obsolete("This class is obsolete; use GridPivotFieldCollection instead")]
public class PivotFields : ICollection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotfields/count/) { get; } | Hämtar antalet element som finns i PivotFields‑instansen |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotfields/issynchronized/) { get; } | Hämtar ett värde som indikerar om åtkomst till PivotFields är synkroniserad (trådsäker). |
| [Item](../../aspose.cells.gridweb.data/pivotfields/item/) { get; } | Hämtar ett PivotField efter index. (2 indexerare) |
| [Parent](../../aspose.cells.gridweb.data/pivotfields/parent/) { get; } | Hämtar föräldraobjektet för det angivna objektet. Skrivskyddad. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotfields/syncroot/) { get; } | Hämtar ett objekt som kan användas för att synkronisera åtkomst till PivotFields. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CopyTo](../../aspose.cells.gridweb.data/pivotfields/copyto/)(Array, int) | Kopierar hela PivotField till en kompatibel endimensionell Array, med start vid det angivna indexet i målarrayen. |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotfields/getenumerator/)() | Returnerar en IEnumerator för PivotFields. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotfields/indexof/)(PivotField) | Hämtar indexet för det angivna PivotField. |

### Anmärkningar

OBS: Den här klassen är nu föråldrad. använd GridPivotFieldCollection istället. Den här klassen kommer att tas bort efter 6 månader från augusti 2014. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp

 [C#]

 //Hämtar PivotFields för PivotTable[0]
 PivotField field1 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field1"];
 PivotField field2 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field2"];
 PivotField field3 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field3"];
 PivotField field4 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field4"];

 //Ställer in plats för PivotFields
 field1.Orientation = PivotFieldOrientation.RowField;
 field2.Orientation = PivotFieldOrientation.RowField;
 field3.Orientation = PivotFieldOrientation.ColumnField;
 field4.Orientation = PivotFieldOrientation.DataField;

 //Ställer in funktion för datafältet
 field3.Function = PivotFieldFunction.Sum;

 //Ändrar ordning på radfält
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

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


