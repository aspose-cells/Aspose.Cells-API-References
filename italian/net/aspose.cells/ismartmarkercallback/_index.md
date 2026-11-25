---
title: "Interfaccia ISmartMarkerCallBack"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Interfaccia Aspose.Cells.ISmartMarkerCallBack. Rappresenta l'interfaccia di callback per l'elaborazione dei smart marker"
type: docs
url: /it/net/aspose.cells/ismartmarkercallback/
---
## ISmartMarkerCallBack interface

Rappresenta l'interfaccia di callback dell'elaborazione di smartmarker.

```csharp
public interface ISmartMarkerCallBack
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Process](../../aspose.cells/ismartmarkercallback/process/)(int, int, int, string, string) | Callback per l'elaborazione di un smart marker. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackDemo : ISmartMarkerCallBack
    {
        // Implementazione del metodo Process dell'interfaccia ISmartMarkerCallBack
        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // Esempio di implementazione del metodo Process
            Console.WriteLine($"Processing sheetIndex: {sheetIndex}, rowIndex: {rowIndex}, colIndex: {colIndex}, tableName: {tableName}, columnName: {columnName}");
        }

        public static void ISmartMarkerCallBackExample()
        {
            // Crea una nuova istanza di WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            // Apri un file modello (che contiene smart marker)
            designer.Workbook = new Workbook("ISmartMarkerCallBackExample_original.xlsx");

            // Imposta l'interfaccia di callback
            designer.CallBack = new ISmartMarkerCallBackDemo();

            // Inizializza i dati dalla fonte dati
            // Per dimostrazione, utilizzeremo una semplice DataTable
            System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Rows.Add("Value1");
            dataTable.Rows.Add("Value2");

            // Imposta la DataTable come fonte dati
            designer.SetDataSource(dataTable);

            // Elabora i smart marker per riempire i dati nei fogli di lavoro
            designer.Process(true);

            // Salva il file Excel
            designer.Workbook.Save("ISmartMarkerCallBackExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


