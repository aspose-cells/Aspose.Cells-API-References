---
title: "OoxmlSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OoxmlSaveOptions-Eigenschaft. Der Datenanbieter zum Speichern der Arbeitsmappe im Light‑Modus"
type: docs
url: /de/net/aspose.cells/ooxmlsaveoptions/lightcellsdataprovider/
---
## OoxmlSaveOptions.LightCellsDataProvider property

Der Datenanbieter zum Speichern der Arbeitsmappe im Light‑Modus.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine benutzerdefinierte LightCellsDataProvider-Implementierung
            var dataProvider = new CustomLightCellsDataProvider();

            // Erstellen Sie Speicheroptionen mit LightCellsDataProvider
            var saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
            {
                LightCellsDataProvider = dataProvider
            };

            // Erstellen Sie eine Arbeitsmappe und speichern Sie sie mit dem Datenanbieter
            var workbook = new Workbook();
            workbook.Save("LightCellsDataProviderDemo.xlsx", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private readonly string[,] data = new string[10, 5]
        {
            {"ID", "Name", "Price", "Qty", "Total"},
            {"1", "Item 1", "10.5", "2", "=B2*C2"},
            {"2", "Item 2", "15.3", "1", "=B3*C3"},
            {"3", "Item 3", "8.2", "5", "=B4*C4"},
            {"4", "Item 4", "12.7", "3", "=B5*C5"},
            {"5", "Item 5", "9.9", "4", "=B6*C6"},
            {"6", "Item 6", "11.2", "2", "=B7*C7"},
            {"7", "Item 7", "14.1", "1", "=B8*C8"},
            {"8", "Item 8", "7.5", "6", "=B9*C9"},
            {"9", "Item 9", "13.4", "2", "=B10*C10"}
        };

        public bool IsGatherString()
        {
            return true;
        }

        public int SheetCount
        {
            get { return 1; }
        }

        public bool StartSheet(int sheetIndex)
        {
            currentRow = -1;
            currentColumn = -1;
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            if (currentRow < data.GetLength(0) - 1)
            {
                currentRow++;
                currentColumn = -1;
                return currentRow;
            }
            return -1;
        }

        public void StartRow(Row row)
        {
            currentColumn = -1;
        }

        public int NextCell()
        {
            if (currentColumn < data.GetLength(1) - 1)
            {
                currentColumn++;
                return currentColumn;
            }
            return -1;
        }

        public void StartCell(Cell cell)
        {
            cell.PutValue(data[currentRow, currentColumn]);
        }

        private int currentRow = -1;
        private int currentColumn = -1;
    }
}
```

### Siehe auch

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


