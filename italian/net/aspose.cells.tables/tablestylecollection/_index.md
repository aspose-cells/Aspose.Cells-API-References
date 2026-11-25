---
title: "Classe TableStyleCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Tables.TableStyleCollection. Rappresenta tutti gli stili di tabella personalizzati"
type: docs
url: /it/net/aspose.cells.tables/tablestylecollection/
---
## TableStyleCollection class

Rappresenta tutti gli stili di tabella personalizzati.

```csharp
public class TableStyleCollection : CollectionBase<TableStyle>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [DefaultPivotStyleName](../../aspose.cells.tables/tablestylecollection/defaultpivotstylename/) { get; set; } | Ottiene e imposta il nome dello stile predefinito della tabella pivot. |
| [DefaultTableStyleName](../../aspose.cells.tables/tablestylecollection/defaulttablestylename/) { get; set; } | Ottiene e imposta il nome dello stile predefinito della tabella. |
| [Item](../../aspose.cells.tables/tablestylecollection/item/) { get; } | Ottiene lo stile della tabella per indice. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddPivotTableStyle](../../aspose.cells.tables/tablestylecollection/addpivottablestyle/)(string) | Aggiunge uno stile personalizzato per tabella pivot. |
| [AddTableStyle](../../aspose.cells.tables/tablestylecollection/addtablestyle/)(string) | Aggiunge uno stile personalizzato per la tabella. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyle) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyle, IComparer&lt;TableStyle&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TableStyle, IComparer&lt;TableStyle&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TableStyle) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyle[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyle[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TableStyle[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TableStyle&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TableStyle&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TableStyle&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TableStyle&gt;) |  |
| [GetBuiltinTableStyle](../../aspose.cells.tables/tablestylecollection/getbuiltintablestyle/)(TableStyleType) | Ottiene lo stile della tabella incorporato |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TablesClassTableStyleCollectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla raccolta degli stili della tabella
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Visualizza i nomi degli stili predefiniti
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Modifica lo stile predefinito della tabella
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            
            // Salva la cartella di lavoro
            workbook.Save("TableStylesDemo.xlsx");
            
            // Verifica la modifica caricando il file salvato
            Workbook verifyWorkbook = new Workbook("TableStylesDemo.xlsx");
            Console.WriteLine("New Default Table Style: " + 
                verifyWorkbook.Worksheets.TableStyles.DefaultTableStyleName);
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TableStyle](../tablestyle/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


