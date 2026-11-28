---
title: "Enum ExternalConnectionClassType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.ExternalConnectionClassType enum. Bağlantı türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnectionclasstype/
---
## ExternalConnectionClassType enumeration

Bağlantı tipini temsil eder.

```csharp
public enum ExternalConnectionClassType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Database | `0` | ODBC veya OLE DB |
| WebQuery | `1` | Web sorgusu |
| TextBased | `2` | Metne göre |
| DataModel | `3` | Veri modeli |
| Unkown | `4` |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassExternalConnectionClassTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bağlantı için örnek veri ekle
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i - 1);
                worksheet.Cells[$"B{i}"].PutValue($"Name_{i - 1}");
            }

            // Veriyle bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Harici bağlantıyı al ve özelliklerini göster
            ExternalConnection conn = workbook.DataConnections[0];
            
            Console.WriteLine($"Connection Name: {conn.Name}");
            Console.WriteLine($"Class Type: {conn.ClassType}");
            Console.WriteLine($"Source Type: {conn.SourceType}");
            Console.WriteLine($"Command: {conn.Command}");
            Console.WriteLine($"Connection File: {conn.ConnectionFile ?? "null"}");
            Console.WriteLine($"Connection String: {conn.ConnectionString ?? "null"}");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


