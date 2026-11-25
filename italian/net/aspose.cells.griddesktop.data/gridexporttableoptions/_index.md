---
title: "Classe GridExportTableOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridDesktop.Data.GridExportTableOptions. Rappresenta tutte le opzioni di esportazione della tabella."
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridexporttableoptions/
---
## GridExportTableOptions class

Rappresenta tutte le opzioni di esportazione della tabella.

```csharp
public class GridExportTableOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridExportTableOptions](gridexporttableoptions/)() | Costruttore di GridExportTableOptions |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CheckMixedValueType](../../aspose.cells.griddesktop.data/gridexporttableoptions/checkmixedvaluetype/) { get; set; } | False, Aspose.Cells imposterà il tipo della DataColumn in base al tipo di valore della prima riga per motivi di prestazioni. True, Aspose.Cells verificherà se il tipo di valore nella colonna è misto prima di impostare il tipo della DataColumn e, se i tipi di valore sono misti, il tipo della DataColumn sarà string. |
| [DataTable](../../aspose.cells.griddesktop.data/gridexporttableoptions/datatable/) { get; set; } | Ottiene e imposta la DataTable a cui è assegnato il tipo di dati delle colonne. |
| [ExportAsHtmlString](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportashtmlstring/) { get; set; } | Esporta il valore stringa HTML delle celle nella DataTable. |
| [ExportAsString](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportasstring/) { get; set; } | Esporta il valore stringa delle celle nella DataTable. |
| [ExportColumnName](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportcolumnname/) { get; set; } | Indica se i dati nella prima riga vengono esportati nel nome della colonna della DataTable. Il valore predefinito è false. |
| [FormatStrategy](../../aspose.cells.griddesktop.data/gridexporttableoptions/formatstrategy/) { get; set; } | Ottiene e imposta la strategia di formattazione quando si esporta il valore come valore stringa. |
| [Indexes](../../aspose.cells.griddesktop.data/gridexporttableoptions/indexes/) { get; set; } | Gli indici delle colonne/righe che devono essere esportati. |
| [IsVertical](../../aspose.cells.griddesktop.data/gridexporttableoptions/isvertical/) { get; set; } | True se una riga nel file Workbook rappresenta una riga nella DataTable. False se una colonna nel file Workbook rappresenta una riga nella DataTable. |
| [PlotVisibleCells](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblecells/) { get; set; } | Esporta solo le celle visibili. |
| [PlotVisibleColumns](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblecolumns/) { get; set; } | Esporta solo le colonne visibili. |
| [PlotVisibleRows](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblerows/) { get; set; } | Esporta solo le righe visibili. |
| [RenameStrategy](../../aspose.cells.griddesktop.data/gridexporttableoptions/renamestrategy/) { get; set; } | Strategia per i nomi duplicati delle colonne. |
| [SkipErrorValue](../../aspose.cells.griddesktop.data/gridexporttableoptions/skiperrorvalue/) { get; set; } | Indica se ignorare i valori non validi per la colonna. Ad esempio, se il tipo della colonna è decimal, il valore è maggiore di decimal.MaxValue e questa proprietà è true, non verrà sollevata nuovamente un'eccezione. Il valore predefinito è false. |

### Vedi anche

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


