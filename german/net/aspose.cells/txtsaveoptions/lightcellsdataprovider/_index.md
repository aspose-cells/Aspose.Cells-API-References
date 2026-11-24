---
title: "TxtSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Der Datenanbieter zum Speichern der Arbeitsmappe im Light‑Modus"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/lightcellsdataprovider/
---
## TxtSaveOptions.LightCellsDataProvider property

Der Datenanbieter zum Speichern der Arbeitsmappe im Light‑Modus.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TxtSaveOptions saveOptions = new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII,
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            string result = SaveAsCsv(workbook, saveOptions);
            Console.WriteLine(result);
        }

        private static string SaveAsCsv(Workbook workbook, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                workbook.Save(stream, options);
                return Encoding.ASCII.GetString(stream.ToArray());
            }
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
            return 1;
        }

        public int NextRow()
        {
            return 1;
        }

        public void StartCell(Cell cell)
        {
            int row = cell.Row;
            int column = cell.Column;
            
            if (row == 0 && column >= 2)
            {
                cell.PutValue($"v_{row + 2}_{column + 2}");
            }
            else if (row > 0 && column >= 2)
            {
                cell.PutValue($"v_{row + 3}_{column + 2}");
            }
        }

        public void StartRow(Row row)
        {
            // Zeileninitialisierung bei Bedarf
        }

        public bool StartSheet(int sheetIndex)
        {
            return sheetIndex == 0;
        }
    }
}
```

### Siehe auch

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


