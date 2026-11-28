---
title: "PivotTable.GetNamesOfSourceDataConnections"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Harici kaynak veri bağlantılarının adlarını alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/
---
## PivotTable.GetNamesOfSourceDataConnections method

Harici kaynak veri bağlantılarının adlarını alır.

```csharp
public string[] GetNamesOfSourceDataConnections()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetNamesOfSourceDataConnectionsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            
            // Pivot tablo oluştur ve referansı al
            int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B3", "C1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Kaynak veri bağlantılarını al
            string[] connections = pivotTable.GetNamesOfSourceDataConnections();
            
            // Bağlantı bilgilerini çıktı olarak ver
            Console.WriteLine("Pivot Table Source Data Connections:");
            foreach (string connection in connections)
            {
                Console.WriteLine(connection);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


