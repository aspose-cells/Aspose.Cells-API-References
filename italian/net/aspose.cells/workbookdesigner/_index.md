---
title: "Class WorkbookDesigner"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WorkbookDesigner. Incapsula l'oggetto che rappresenta un foglio di calcolo designer"
type: docs
url: /it/net/aspose.cells/workbookdesigner/
---
## WorkbookDesigner class

Incapsula l'oggetto che rappresenta un foglio di calcolo di progettazione.

```csharp
public class WorkbookDesigner
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WorkbookDesigner](workbookdesigner/#constructor)() | Inizializza una nuova istanza della classe `WorkbookDesigner`. |
| [WorkbookDesigner](workbookdesigner/#constructor_1)(Workbook) | Inizializza una nuova istanza della classe `WorkbookDesigner`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula/) { get; set; } | Indica se le formule devono essere calcolate. |
| [CallBack](../../aspose.cells/workbookdesigner/callback/) { get; set; } | Ottiene e imposta l'interfaccia di callback dell'elaborazione di smartmarker. |
| [ContainsVariables](../../aspose.cells/workbookdesigner/containsvariables/) { get; set; } | (**Obsolete.**) Indica se il primo foglio di lavoro contiene variabili personalizzate. |
| [EnableHeaderFooterMarkers](../../aspose.cells/workbookdesigner/enableheaderfootermarkers/) { get; set; } | Indica se intestazione/piè di pagina contiene smart marker e deve essere elaborato insieme. |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline/) { get; set; } | (**Obsolete.**) Indica se l'elaborazione del smart marker avviene riga per riga. |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal/) { get; set; } | Indica se le formule vengono ripetute con la riga di subtotale. |
| [SortDataSource](../../aspose.cells/workbookdesigner/sortdatasource/) { get; set; } | Indica se l'origine dati è ordinata. |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull/) { get; set; } | Se TRUE, verrà inserito Null se il valore è ""; |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference/) { get; set; } | Indica se i riferimenti in altri fogli di lavoro verranno aggiornati. |
| [VariablesWorksheetName](../../aspose.cells/workbookdesigner/variablesworksheetname/) { get; set; } | Ottiene e imposta il nome del foglio di lavoro che contiene variabili smart marker. |
| [Workbook](../../aspose.cells/workbookdesigner/workbook/) { get; set; } | Ottiene e imposta l'oggetto [`Workbook`](./workbook/). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource/)() | Cancella tutte le origini dati. |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers/)() | Restituisce una raccolta di smart marker in un foglio di calcolo. |
| [Process](../../aspose.cells/workbookdesigner/process/#process)() | Elabora gli smart marker e popola i valori dell'origine dati. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_2)(bool) | Elabora gli smart marker e popola i valori dell'origine dati. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_3)(int, bool) | Elabora gli smart marker e popola i valori dell'origine dati. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_1)(Range, bool) | (**Obsolete.**) Elabora gli smart marker e popola i valori dell'origine dati. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource)(DataSet) | Imposta l'origine dati di un oggetto DataSet. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_1)(DataTable) | Imposta l'origine dati di un oggetto DataTable. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_2)(DataView) | Imposta l'origine dati di un oggetto DataView. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_3)(OleDbConnection) | Imposta l'origine dati di un oggetto OleDbConnection. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_4)(SqlConnection) | Imposta l'origine dati di un oggetto SqlConnection. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_6)(string, DataView) | Imposta l'origine dati di un oggetto DataView e lo associa a un nome di origine dati. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_5)(string, ICellsDataTable) | Imposta l'origine dati di un oggetto [`ICellsDataTable`](../icellsdatatable/). |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_8)(string, object) | Imposta il binding dei dati a una variabile. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_7)(string, IDataReader, int) | Imposta l'origine dati di un oggetto IDataReader. |
| [SetJsonDataSource](../../aspose.cells/workbookdesigner/setjsondatasource/)(string, string) | Imposta il valore della stringa JSON come origine dati degli smart marker. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerDemo
    {
        public static void WorkbookDesignerExample()
        {
            // Crea l'oggetto WorkbookDesigner
            WorkbookDesigner wd = new WorkbookDesigner();

            // Apri il file modello (che contiene smart marker)
            wd.Workbook = new Workbook("SmartMarker_Designer_original.xlsx");

            // Inizializza i dati dalla fonte dati
            DataSet ds = new DataSet();
            // Aggiungi dati al dataset (questo è solo un esempio, sostituisci con l'origine dati reale)
            DataTable dt = new DataTable("Table1");
            dt.Columns.Add("Column1");
            dt.Columns.Add("Column2");
            dt.Rows.Add("Value1", "Value2");
            dt.Rows.Add("Value11", "Value22");
            ds.Tables.Add(dt);

            // Imposta il dataset come origine dati
            wd.SetDataSource(ds);

            // Elabora i smart marker per riempire i dati nei fogli di lavoro
            wd.Process(true);

            // Salva il file Excel
            wd.Workbook.Save("WorkbookDesignerExample.xlsx");

            // Dimostrazione di altre proprietà
            wd.RepeatFormulasWithSubtotal = true;
            wd.UpdateEmptyStringAsNull = true;
            wd.UpdateReference = true;
            wd.CalculateFormula = true;
            wd.LineByLine = true;

            // Cancella l'origine dati
            wd.ClearDataSource();

            // Imposta l'origine dati usando metodi diversi
            wd.SetDataSource("dataSourceName", dt);
            wd.SetDataSource(dt);
            wd.SetDataSource(ds);
            wd.SetDataSource("dataSourceName", new DataView(dt));
            wd.SetDataSource(new DataView(dt));
            wd.SetDataSource("name", new DataTableReader(dt), dt.Rows.Count);
            wd.SetJsonDataSource("variable", "{\"key\":\"value\"}");
            wd.SetDataSource("variable", new object());

            // Elabora nuovamente gli smart marker
            wd.Process();
            wd.Process(true);
            wd.Process(0, true);

            // Salva nuovamente il file Excel
            wd.Workbook.Save("WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


