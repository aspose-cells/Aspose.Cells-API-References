---
title: "Schnittstelle ISmartMarkerCallBack"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ISmartMarkerCallBack Schnittstelle. Stellt die Rückruffunktion für die Verarbeitung von Smartmarker dar."
type: docs
url: /de/net/aspose.cells/ismartmarkercallback/
---
## ISmartMarkerCallBack interface

Stellt die Callback‑Schnittstelle für die Verarbeitung von Smartmarker dar.

```csharp
public interface ISmartMarkerCallBack
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Process](../../aspose.cells/ismartmarkercallback/process/)(int, int, int, string, string) | Rückruf für die Verarbeitung eines Smartmarkers. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackDemo : ISmartMarkerCallBack
    {
        // Implementierung der Process‑Methode aus der ISmartMarkerCallBack‑Schnittstelle
        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // Beispielhafte Implementierung der Process‑Methode
            Console.WriteLine($"Processing sheetIndex: {sheetIndex}, rowIndex: {rowIndex}, colIndex: {colIndex}, tableName: {tableName}, columnName: {columnName}");
        }

        public static void ISmartMarkerCallBackExample()
        {
            // Erstellen Sie eine neue WorkbookDesigner‑Instanz
            WorkbookDesigner designer = new WorkbookDesigner();
            // Öffnen Sie eine Vorlagendatei (die Smartmarker enthält)
            designer.Workbook = new Workbook("ISmartMarkerCallBackExample_original.xlsx");

            // Setzen Sie die Rückruf‑Schnittstelle
            designer.CallBack = new ISmartMarkerCallBackDemo();

            // Initialisieren Sie Ihre Daten aus der Datenquelle
            // Zur Demonstration verwenden wir eine einfache DataTable
            System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Rows.Add("Value1");
            dataTable.Rows.Add("Value2");

            // Legen Sie die DataTable als Datenquelle fest
            designer.SetDataSource(dataTable);

            // Verarbeiten Sie die Smartmarker, um die Daten in die Arbeitsblätter einzufügen
            designer.Process(true);

            // Speichere die Excel-Datei
            designer.Workbook.Save("ISmartMarkerCallBackExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


