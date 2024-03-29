---
title: OoxmlSaveOptions
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta le opzioni di salvataggio del file xml aperto di Office.
type: docs
weight: 4370
url: /it/net/aspose.cells/ooxmlsaveoptions/
---
## OoxmlSaveOptions class

Rappresenta le opzioni di salvataggio del file xml aperto di Office.

```csharp
public class OoxmlSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [OoxmlSaveOptions](ooxmlsaveoptions#constructor)() | Crea le opzioni per salvare il file xml aperto di Office. |
| [OoxmlSaveOptions](ooxmlsaveoptions#constructor_1)(SaveFormat) | Crea le opzioni per salvare il file xml aperto di Office. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | La cartella dei file nella cache viene utilizzata per memorizzare dati di grandi dimensioni. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Rendi vuota la cartella di lavoro dopo aver salvato il file. |
| [CompressionType](../../aspose.cells/ooxmlsaveoptions/compressiontype) { get; set; } | Ottiene e imposta il tipo di compressione per il file ooxml. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [EmbedOoxmlAsOleObject](../../aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject) { get; set; } | Indica se incorporare file Ooxml di OleObject come oggetto ole. |
| [EnableZip64](../../aspose.cells/ooxmlsaveoptions/enablezip64) { get; set; } | Usa sempre le estensioni ZIP64 quando scrivi archivi zip, anche quando non necessario. |
| [ExportCellName](../../aspose.cells/ooxmlsaveoptions/exportcellname) { get; set; } | Indica se esportare il nome della cella nel file Excel2007 .xlsx (.xlsm, .xltx, .xltm). Se è possibile accedere al file di output da SQL Server DTS, questo valore deve essere true. L'impostazione del valore su false aumenterà notevolmente le prestazioni e ridurrà le dimensioni del file durante la creazione di file di grandi dimensioni. Il valore predefinito è true. |
| [LightCellsDataProvider](../../aspose.cells/ooxmlsaveoptions/lightcellsdataprovider) { get; set; } | Il provider di dati per fornire i dati delle celle per il salvataggio della cartella di lavoro in modalità luce. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Indica se unire le aree di formattazione condizionale e validazione prima di salvare il file. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indica se aggiornare i dati della cache del grafico |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Ottiene il formato del file di salvataggio. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indica se aggiornare l'impostazione Smart Art. Il valore predefinito è false. |
| [UpdateZoom](../../aspose.cells/ooxmlsaveoptions/updatezoom) { get; set; } | Indica se aggiornare il fattore di scala prima di salvare il file se le proprietà PageSetup.FitToPagesWide e PageSetup.FitToPagesTall controllano la modalità di ridimensionamento del foglio di lavoro. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Ottiene o imposta la richiamata di avviso. |

### Guarda anche

* class [SaveOptions](../saveoptions)
* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
