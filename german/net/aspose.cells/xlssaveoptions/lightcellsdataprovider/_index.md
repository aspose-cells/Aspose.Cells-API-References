---
title: "XlsSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XlsSaveOptions-Eigenschaft. Der Datenanbieter zum Speichern der Arbeitsmappe im Light-Modus"
type: docs
url: /de/net/aspose.cells/xlssaveoptions/lightcellsdataprovider/
---
## XlsSaveOptions.LightCellsDataProvider property

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
    public class XlsSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // XLS-Speicheroptionen erstellen
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            
            // Den LightCellsDataProvider festlegen
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
            
            // Speichern Sie die Arbeitsmappe im LightCells-Modus
            workbook.Save("output.xls", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        public bool IsGatherString()
        {
            return true;
        }

        public int NextCell()
        {
            return 0; // Only process first cell for demonstration
        }

        public int NextRow()
        {
            return 0; // Only process first row for demonstration
        }

        public void StartCell(Cell cell)
        {
            // Setzen Sie einen langen Zeichenfolgenwert, um die Handhabung von LightCells zu demonstrieren
            cell.PutValue(new string('X', 257));
        }

        public void StartRow(Row row)
        {
            // Keine spezielle Zeilenverarbeitung für diese Demo erforderlich
        }

        public bool StartSheet(int sheetIndex)
        {
            // Keine spezielle Blattverarbeitung für diese Demo erforderlich
            return false;
        }
    }
}
```

### Siehe auch

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


