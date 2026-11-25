---
title: "Classe ListObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Tables.ListObject. Rappresenta una tabella in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells.tables/listobject/
---
## ListObject class

Rappresenta una tabella in un foglio di lavoro.

```csharp
public class ListObject
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription/) { get; set; } | Ottiene e imposta la descrizione alternativa. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext/) { get; set; } | Ottiene e imposta il testo alternativo. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter/) { get; } | Ottiene il filtro automatico di questa tabella. |
| [Comment](../../aspose.cells.tables/listobject/comment/) { get; set; } | Ottiene e imposta il commento della tabella. |
| [DataRange](../../aspose.cells.tables/listobject/datarange/) { get; } | Ottiene l'intervallo di dati della Tabella. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype/) { get; } | Ottiene il tipo di origine dati della tabella. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname/) { get; set; } | Ottiene e imposta il nome visualizzato della tabella. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn/) { get; } | Ottiene la colonna finale dell'intervallo. |
| [EndRow](../../aspose.cells.tables/listobject/endrow/) { get; } | Ottiene la riga finale dell'intervallo. |
| [HasAutoFilter](../../aspose.cells.tables/listobject/hasautofilter/) { get; set; } | Indica se il filtro automatico è applicato a questa tabella. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns/) { get; } | Ottiene l'elenco [`ListColumn`](../listcolumn/) di questa tabella. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable/) { get; } | Ottiene la QueryTable collegata. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow/) { get; set; } | Ottiene e imposta se questa Tabella mostra la riga di intestazione. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes/) { get; set; } | Indica se la formattazione a strisce di colonna è applicata a. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn/) { get; set; } | Indica se la prima colonna nella tabella è lo stile applicato a. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn/) { get; set; } | Indica se l'ultima colonna nella tabella è lo stile applicato a. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes/) { get; set; } | Indica se la formattazione a strisce di riga è applicata a. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals/) { get; set; } | Ottiene e imposta se questa TAble mostra la riga totale. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn/) { get; } | Ottiene la colonna iniziale dell'intervallo. |
| [StartRow](../../aspose.cells.tables/listobject/startrow/) { get; } | Ottiene la riga iniziale dell'intervallo. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename/) { get; set; } | Ottiene e imposta il nome dello stile della tabella. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype/) { get; set; } | Ottiene e lo stile di tabella incorporato. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap/) { get; } | Ottiene un [`XmlMap`](./xmlmap/) usato per questo elenco. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange/)() | Applica lo stile di tabella all'intervallo. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange)() | Converti la tabella in intervallo. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange_1)(TableToRangeOptions) | Converti la tabella in intervallo. |
| [Filter](../../aspose.cells.tables/listobject/filter/)() | (**Obsoleto.**) Filtra la tabella. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula)(int, int, string) | Inserisci la formula nella cella della tabella. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula_1)(int, int, string, bool) | Inserisci la formula nella cella della tabella. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue)(int, int, object) | Inserisci il valore nella cella. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue_1)(int, int, object, bool) | Inserisci il valore nella cella. |
| [RemoveAutoFilter](../../aspose.cells.tables/listobject/removeautofilter/)() | Rimuove il filtro automatico applicato a questa tabella. |
| [Resize](../../aspose.cells.tables/listobject/resize/)(int, int, int, int, bool) | Ridimensiona l'intervallo dell'oggetto elenco. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname/)() | Aggiorna i nomi di tutte le colonne dell'elenco nelle celle della tabella. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectDemo
    {
        public static void ListObjectExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola il foglio di lavoro con alcuni dati
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Aggiungi un ListObject (tabella) al foglio di lavoro
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Imposta alcune proprietà del ListObject
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
            table.DisplayName = "SampleTable";
            table.Comment = "This is a sample table.";
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.ShowTableStyleRowStripes = true;
            table.ShowTableStyleColumnStripes = true;
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Salva la cartella di lavoro
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


