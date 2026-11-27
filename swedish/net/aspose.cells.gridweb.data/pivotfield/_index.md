---
title: "Klass PivotField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.PivotField-klass. Representerar ett fält i en PivotTable-rapport. PivotField-objektet är en medlem i PivotFields-samlingen.  OBS Denna klass är nu föråldrad. Använd istället GridPivotField. Klassen kommer att tas bort efter 6 månader från augusti 2014. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt."
type: docs
url: /sv/net/aspose.cells.gridweb.data/pivotfield/
---
## PivotField class

Representerar ett fält i en PivotTable-rapport. PivotField-objektet är en medlem i [`PivotFields`](../pivotfields/) samlingen.  OBS: Denna klass är nu föråldrad. Använd istället GridPivotField. Klassen kommer att tas bort efter 6 månader från augusti 2014. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

```csharp
[Obsolete("This class is obsolete; use GridPivotField instead")]
public class PivotField
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Caption](../../aspose.cells.gridweb.data/pivotfield/caption/) { get; set; } | Etiketttexten för pivotfältet visas i rapporten. Som standard visas namnet. |
| [FieldItems](../../aspose.cells.gridweb.data/pivotfield/fielditems/) { get; } | Hämtar data för det angivna fältet. |
| [Function](../../aspose.cells.gridweb.data/pivotfield/function/) { get; set; } | Representerar funktionen som används för att sammanfatta PivotTable-fältet (endast datafält). Standardfunktionen är Count. |
| [Name](../../aspose.cells.gridweb.data/pivotfield/name/) { get; } | Hämtar namnet. |
| [Orientation](../../aspose.cells.gridweb.data/pivotfield/orientation/) { get; set; } | Representerar platsen för fältet i den angivna PivotTable‑rapporten. |
| [Position](../../aspose.cells.gridweb.data/pivotfield/position/) { get; set; } | Representerar positionen för fältet (första, andra, tredje osv.) bland alla fält i dess orientering (Rows, Columns, Pages). Du bör anropa get‑metoden efter att ha anropat Pivottable.DataBind. |
| [SortOrder](../../aspose.cells.gridweb.data/pivotfield/sortorder/) { get; set; } | Representerar den ordning som används för att sortera det angivna PivotTable‑fältet. |

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


