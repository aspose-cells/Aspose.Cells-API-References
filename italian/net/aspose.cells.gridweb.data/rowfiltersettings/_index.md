---
title: "Classe RowFilterSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.RowFilterSettings. Descrizione riepilogativa per RowFilter"
type: docs
url: /it/net/aspose.cells.gridweb.data/rowfiltersettings/
---
## RowFilterSettings class

Descrizione riepilogativa per RowFilter.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet.AddAutoFilter/FilterString for autofilter /custom filter settings")]
public class RowFilterSettings : IComparer, ISerializable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Criteria](../../aspose.cells.gridweb.data/rowfiltersettings/criteria/) { get; set; } | La stringa dei criteri di filtro. |
| [EnableAutoFilter](../../aspose.cells.gridweb.data/rowfiltersettings/enableautofilter/) { get; set; } | Abilita il filtro automatico. L'HeaderRow mostrerà pulsanti a discesa per consentire all'utente di selezionare il valore della colonna da filtrare. |
| [EndColumn](../../aspose.cells.gridweb.data/rowfiltersettings/endcolumn/) { get; set; } | Il numero della riga finale dell'intervallo di filtro. Se questo valore è impostato a -1, viene usato l'ultimo numero di riga del foglio. |
| [HeaderRow](../../aspose.cells.gridweb.data/rowfiltersettings/headerrow/) { get; set; } | Il numero della riga di intestazione che mostrerà i pulsanti a discesa del filtro. |
| [StartColumn](../../aspose.cells.gridweb.data/rowfiltersettings/startcolumn/) { get; set; } | Il numero della riga iniziale dell'intervallo di filtro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [BuildAutoFilterCriteria](../../aspose.cells.gridweb.data/rowfiltersettings/buildautofiltercriteria/)() | Crea la stringa dei criteri dalle impostazioni del filtro automatico. |
| [ClearFilter](../../aspose.cells.gridweb.data/rowfiltersettings/clearfilter/)() | Cancella tutte le impostazioni di filtro e visualizza tutte le righe. |
| [CustomFilter](../../aspose.cells.gridweb.data/rowfiltersettings/customfilter/)(int, ICustomFilter) | Specifica un filtro personalizzato. |
| [FilterRows](../../aspose.cells.gridweb.data/rowfiltersettings/filterrows/)() | Filtra le righe usando la stringa dei criteri. |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Questa classe sarà rimossa dopo 6 mesi da agosto 2014. È possibile utilizzare GridWorksheet AddAutoFilter/FilterString per le impostazioni di filtro automatico/personalizzato. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


