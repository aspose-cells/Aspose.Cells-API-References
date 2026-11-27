---
title: "Klass SqlScriptSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Saving.SqlScriptSaveOptions klass. Representerar alternativen för att spara sql"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions class

Representerar alternativen för att spara sql.

```csharp
public class SqlScriptSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SqlScriptSaveOptions](sqlscriptsaveoptions/)() | Skapar alternativ för att spara sql‑fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AddBlankLineBetweenRows](../../aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/) { get; set; } | Infoga en tom rad mellan varje data. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckAllDataForColumnType](../../aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/) { get; set; } | Kontrollera all data för att hitta kolumnernas datatyp. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner i Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckIfTableExists](../../aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/) { get; set; } | Kontrollera om tabellnamnet finns innan det skapas |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ColumnTypeMap](../../aspose.cells.saving/sqlscriptsaveoptions/columntypemap/) { get; set; } | Hämtar och anger mappningen av kolumntyp för olika databaser. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns kommer katalogen att skapas automatiskt innan filen sparas. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateTable](../../aspose.cells.saving/sqlscriptsaveoptions/createtable/) { get; set; } | Indikerar om sql för att skapa tabell exporteras. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras vid sparande som .xls-fil. Standardvärdet är sant.(Ärvd från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExportArea](../../aspose.cells.saving/sqlscriptsaveoptions/exportarea/) { get; set; } | Hämtar eller anger exportintervallet. |
| [ExportAsString](../../aspose.cells.saving/sqlscriptsaveoptions/exportasstring/) { get; set; } | Indikerar om all data exporteras som strängvärde. |
| [HasHeaderRow](../../aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/) { get; set; } | Anger om intervallet innehåller en rubrikrad. |
| [IdName](../../aspose.cells.saving/sqlscriptsaveoptions/idname/) { get; set; } | Hämtar och anger namnet på id‑kolumnen. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås samman innan filen sparas.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [OperatorType](../../aspose.cells.saving/sqlscriptsaveoptions/operatortype/) { get; set; } | Hämtar och anger operator‑typen för sql. |
| [PrimaryKey](../../aspose.cells.saving/sqlscriptsaveoptions/primarykey/) { get; set; } | Representerar vilken kolumn som är primärnyckel i datatabellen. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste datan för diagrammet ska cachas.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar filformatet för sparning.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [Separator](../../aspose.cells.saving/sqlscriptsaveoptions/separator/) { get; set; } | Hämtar och anger teckenseparatorn för sql‑skriptet. |
| [SheetIndexes](../../aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/) { get; set; } | Representerar indexen för exporterade blad. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [StartId](../../aspose.cells.saving/sqlscriptsaveoptions/startid/) { get; set; } | Hämtar och anger start‑id. |
| [TableName](../../aspose.cells.saving/sqlscriptsaveoptions/tablename/) { get; set; } | Hämtar och anger tabellnamnet. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art uppdateras. Standardvärdet är false.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varnings‑callback.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll kalkylbladet med lite data
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Name");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue("John Doe");
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("Jane Doe");

            // Skapa en instans av SqlScriptSaveOptions
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

            // Spara arbetsboken som SQL-skript
            workbook.Save("MyTable.sql", saveOptions);

            return;
        }
    }
}
```

### Se även

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


