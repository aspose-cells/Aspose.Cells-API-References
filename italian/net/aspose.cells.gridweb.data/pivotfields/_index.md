---
title: "Classe PivotFields"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridWeb.Data.PivotFields class. Rappresenta una raccolta di tutti gli oggetti PivotField in un report PivotTable"
type: docs
url: /it/net/aspose.cells.gridweb.data/pivotfields/
---
## PivotFields class

Rappresenta una raccolta di tutti gli oggetti [`PivotField`](../pivotfield/) in un report PivotTable.

```csharp
[Obsolete("This class is obsolete; use GridPivotFieldCollection instead")]
public class PivotFields : ICollection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotfields/count/) { get; } | Ottiene il numero di elementi contenuti nell'istanza PivotFields |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotfields/issynchronized/) { get; } | Ottiene un valore che indica se l'accesso a PivotFields è sincronizzato (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/pivotfields/item/) { get; } | Ottiene un PivotField per indice. (2 indicizzatori) |
| [Parent](../../aspose.cells.gridweb.data/pivotfields/parent/) { get; } | Ottiene l'oggetto padre per l'oggetto specificato. Sola lettura. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotfields/syncroot/) { get; } | Ottiene un oggetto che può essere usato per sincronizzare l'accesso a PivotFields. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CopyTo](../../aspose.cells.gridweb.data/pivotfields/copyto/)(Array, int) | Copia l'intero PivotField in un Array monodimensionale compatibile, iniziando all'indice specificato dell'array di destinazione. |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotfields/getenumerator/)() | Restituisce un IEnumerator per PivotFields. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotfields/indexof/)(PivotField) | Ottiene l'indice del PivotField specificato. |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Si prega di utilizzare GridPivotFieldCollection invece. Questa classe sarà rimossa dopo 6 mesi da agosto 2014. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp

 [C#]

 //Ottiene i PivotFields di PivotTable[0]
 PivotField field1 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field1"];
 PivotField field2 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field2"];
 PivotField field3 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field3"];
 PivotField field4 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field4"];

 //Imposta la posizione di PivotFields
 field1.Orientation = PivotFieldOrientation.RowField;
 field2.Orientation = PivotFieldOrientation.RowField;
 field3.Orientation = PivotFieldOrientation.ColumnField;
 field4.Orientation = PivotFieldOrientation.DataField;

 //Imposta la funzione del campo dati
 field3.Function = PivotFieldFunction.Sum;

 //Modifica l'ordine dei campi della riga
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

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


