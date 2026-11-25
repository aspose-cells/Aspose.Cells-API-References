---
title: "Classe PivotField"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.PivotField. Rappresenta un campo in un report PivotTable. L'oggetto PivotField è un membro della raccolta PivotFields. NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare GridPivotField. Questa classe sarà rimossa dopo 6 mesi da agosto 2014. Aspose si scusa per eventuali disagi che potresti aver riscontrato"
type: docs
url: /it/net/aspose.cells.gridweb.data/pivotfield/
---
## PivotField class

Rappresenta un campo in un report PivotTable. L'oggetto PivotField è un membro della raccolta [`PivotFields`](../pivotfields/). NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare GridPivotField. Questa classe sarà rimossa dopo 6 mesi da agosto 2014. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

```csharp
[Obsolete("This class is obsolete; use GridPivotField instead")]
public class PivotField
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Caption](../../aspose.cells.gridweb.data/pivotfield/caption/) { get; set; } | Il testo dell'etichetta per il campo pivot viene mostrato nel report. Per impostazione predefinita mostra il nome. |
| [FieldItems](../../aspose.cells.gridweb.data/pivotfield/fielditems/) { get; } | Restituisce i dati del campo specificato. |
| [Function](../../aspose.cells.gridweb.data/pivotfield/function/) { get; set; } | Rappresenta la funzione utilizzata per riepilogare il campo PivotTable (solo campi dati). La funzione predefinita è Count. |
| [Name](../../aspose.cells.gridweb.data/pivotfield/name/) { get; } | Restituisce il nome. |
| [Orientation](../../aspose.cells.gridweb.data/pivotfield/orientation/) { get; set; } | Rappresenta la posizione del campo nel report PivotTable specificato. |
| [Position](../../aspose.cells.gridweb.data/pivotfield/position/) { get; set; } | Rappresenta la posizione del campo (primo, secondo, terzo, ecc.) tra tutti i campi nella sua orientazione (Righe, Colonne, Pagine). È necessario chiamare il metodo get dopo aver chiamato Pivottable.DataBind. |
| [SortOrder](../../aspose.cells.gridweb.data/pivotfield/sortorder/) { get; set; } | Rappresenta l'ordine utilizzato per ordinare il campo PivotTable specificato. |

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


