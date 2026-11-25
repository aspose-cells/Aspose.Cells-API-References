---
title: "Class OoxmlSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.OoxmlSaveOptions. Rappresenta le opzioni per salvare un file Office Open XML."
type: docs
url: /it/net/aspose.cells/ooxmlsaveoptions/
---
## OoxmlSaveOptions class

Rappresenta le opzioni di salvataggio del file Office Open XML.

```csharp
public class OoxmlSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [OoxmlSaveOptions](ooxmlsaveoptions/#constructor)() | Crea le opzioni per salvare un file Office Open XML. |
| [OoxmlSaveOptions](ooxmlsaveoptions/#constructor_1)(SaveFormat) | Crea le opzioni per salvare un file Office Open XML. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AsFlatOpc](../../aspose.cells/ooxmlsaveoptions/asflatopc/) { get; set; } | Indica se salvare come file OPC piatto che può essere generato dall'Open XML SDK. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendi il workbook vuoto dopo aver salvato il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CompressionType](../../aspose.cells/ooxmlsaveoptions/compressiontype/) { get; set; } | Ottiene e imposta il tipo di compressione per il file ooxml. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [EmbedOoxmlAsOleObject](../../aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/) { get; set; } | Indica se incorporare i file Ooxml di OleObject come oggetto OLE. |
| [EnableZip64](../../aspose.cells/ooxmlsaveoptions/enablezip64/) { get; set; } | Usa le estensioni ZIP64 quando scrivi archivi zip, se necessario. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ExportCellName](../../aspose.cells/ooxmlsaveoptions/exportcellname/) { get; set; } | Indica se esportare il nome della cella in un file Excel2007 .xlsx (.xlsm, .xltx, .xltm). Se il file di output può essere accessibile da SQL Server DTS, questo valore deve essere true. Impostare il valore a false aumenterà notevolmente le prestazioni e ridurrà le dimensioni del file quando si crea un file di grandi dimensioni. Il valore predefinito è true. |
| [LightCellsDataProvider](../../aspose.cells/ooxmlsaveoptions/lightcellsdataprovider/) { get; set; } | Il provider di dati per salvare la cartella di lavoro in modalità leggera. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica se aggiornare le impostazioni di smart art. Il valore predefinito è false. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [UpdateZoom](../../aspose.cells/ooxmlsaveoptions/updatezoom/) { get; set; } | Indica se aggiornare il fattore di scala prima di salvare il file se le proprietà PageSetup.FitToPagesWide e PageSetup.FitToPagesTall controllano come il foglio di lavoro viene scalato. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ottiene o imposta la callback di avviso.(Ereditato da [`SaveOptions`](../saveoptions/).) |
| [WpsCompatibility](../../aspose.cells/ooxmlsaveoptions/wpscompatibility/) { get; set; } | (**Obsolete.**) Indica se rendere il file xls più compatibile con WPS. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsDemo
    {
        public static void OoxmlSaveOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci alcuni dati nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Crea un'istanza di OoxmlSaveOptions
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

            // Impostazione delle proprietà
            saveOptions.ExportCellName = true;
            saveOptions.UpdateZoom = true;
            saveOptions.EnableZip64 = false;
            saveOptions.EmbedOoxmlAsOleObject = false;
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = "C:\\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Salva la cartella di lavoro con le opzioni specificate
            workbook.Save("OoxmlSaveOptionsExample.xlsx", saveOptions);

            return;
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


