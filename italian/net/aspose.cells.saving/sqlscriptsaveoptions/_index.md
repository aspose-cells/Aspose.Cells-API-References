---
title: "Classe SqlScriptSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Saving.SqlScriptSaveOptions. Rappresenta le opzioni di salvataggio SQL"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions class

Rappresenta le opzioni di salvataggio di sql.

```csharp
public class SqlScriptSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SqlScriptSaveOptions](sqlscriptsaveoptions/)() | Crea le opzioni per il salvataggio del file SQL. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AddBlankLineBetweenRows](../../aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/) { get; set; } | Inserisci una riga vuota tra ogni dato. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckAllDataForColumnType](../../aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/) { get; set; } | Controlla tutti i dati per trovare il tipo di dato delle colonne. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, excel non consente di inserire una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, verrà troncato.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckIfTableExists](../../aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/) { get; set; } | Verifica se il nome della tabella esiste prima di crearla |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rende la cartella di lavoro vuota dopo aver salvato il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ColumnTypeMap](../../aspose.cells.saving/sqlscriptsaveoptions/columntypemap/) { get; set; } | Ottiene e imposta la mappa del tipo di colonna per diversi database. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateTable](../../aspose.cells.saving/sqlscriptsaveoptions/createtable/) { get; set; } | Indica se esportare SQL per la creazione della tabella. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExportArea](../../aspose.cells.saving/sqlscriptsaveoptions/exportarea/) { get; set; } | Ottiene o imposta l'intervallo di esportazione. |
| [ExportAsString](../../aspose.cells.saving/sqlscriptsaveoptions/exportasstring/) { get; set; } | Indica se esportare tutti i dati come valore stringa. |
| [HasHeaderRow](../../aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/) { get; set; } | Indica se l'intervallo contiene la riga di intestazione. |
| [IdName](../../aspose.cells.saving/sqlscriptsaveoptions/idname/) { get; set; } | Ottiene e imposta il nome della colonna ID. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [OperatorType](../../aspose.cells.saving/sqlscriptsaveoptions/operatortype/) { get; set; } | Ottiene e imposta il tipo di operatore SQL. |
| [PrimaryKey](../../aspose.cells.saving/sqlscriptsaveoptions/primarykey/) { get; set; } | Rappresenta quale colonna è la chiave primaria della tabella dati. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [Separator](../../aspose.cells.saving/sqlscriptsaveoptions/separator/) { get; set; } | Ottiene e imposta il separatore di caratteri dello script SQL. |
| [SheetIndexes](../../aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/) { get; set; } | Rappresenta gli indici dei fogli esportati. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [StartId](../../aspose.cells.saving/sqlscriptsaveoptions/startid/) { get; set; } | Ottiene e imposta l'ID iniziale. |
| [TableName](../../aspose.cells.saving/sqlscriptsaveoptions/tablename/) { get; set; } | Ottiene e imposta il nome della tabella. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica se aggiornare l'impostazione SmartArt. Il valore predefinito è false.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ottiene o imposta il callback di avviso.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptSaveOptionsDemo
    {
        public static void SqlScriptSaveOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Riempie il foglio di lavoro con alcuni dati
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Name");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue("John Doe");
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("Jane Doe");

            // Crea un'istanza di SqlScriptSaveOptions
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                ColumnTypeMap = new SqlScriptColumnTypeMap(),
                CheckAllDataForColumnType = true,
                AddBlankLineBetweenRows = false,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "MyTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                WarningCallback = null,
                UpdateSmartArt = false
            };

            // Salva la cartella di lavoro come script SQL.
            workbook.Save("MyTable.sql", saveOptions);

            return;
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


