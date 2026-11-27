---
title: "Gränssnitt ISmartMarkerCallBack"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ISmartMarkerCallBack-gränssnitt. Representerar återuppringningsgränssnitt för bearbetning av smartmarker"
type: docs
url: /sv/net/aspose.cells/ismartmarkercallback/
---
## ISmartMarkerCallBack interface

Representerar återuppringningsgränssnittet för bearbetning av smartmarker.

```csharp
public interface ISmartMarkerCallBack
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Process](../../aspose.cells/ismartmarkercallback/process/)(int, int, int, string, string) | Återuppringning för bearbetning av en smart marker. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackDemo : ISmartMarkerCallBack
    {
        // Implementering av Process‑metoden från ISmartMarkerCallBack‑gränssnittet
        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // Exempel på implementering av Process‑metoden
            Console.WriteLine($"Processing sheetIndex: {sheetIndex}, rowIndex: {rowIndex}, colIndex: {colIndex}, tableName: {tableName}, columnName: {columnName}");
        }

        public static void ISmartMarkerCallBackExample()
        {
            // Skapa en ny WorkbookDesigner‑instans
            WorkbookDesigner designer = new WorkbookDesigner();
            // Öppna en mallfil (som innehåller smart markers)
            designer.Workbook = new Workbook("ISmartMarkerCallBackExample_original.xlsx");

            // Ställ in återuppringningsgränssnittet
            designer.CallBack = new ISmartMarkerCallBackDemo();

            // Initiera dina data från datakällan
            // För demonstration kommer vi att använda en enkel DataTable
            System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Rows.Add("Value1");
            dataTable.Rows.Add("Value2");

            // Ange datatabellen som datakälla
            designer.SetDataSource(dataTable);

            // Bearbeta smart markers för att fylla i data i kalkylbladen
            designer.Process(true);

            // Spara Excel-filen
            designer.Workbook.Save("ISmartMarkerCallBackExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


