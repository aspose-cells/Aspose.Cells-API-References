---
title: "Enum ConnectionDataSourceType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.ConnectionDataSourceType enum. Harici veritabanı kaynağı türünü belirtir"
type: docs
url: /tr/net/aspose.cells.externalconnections/connectiondatasourcetype/
---
## ConnectionDataSourceType enumeration

Harici veritabanı kaynak türünü belirtir

```csharp
public enum ConnectionDataSourceType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| ODBCBasedSource | `1` | ODBC tabanlı kaynak |
| DAOBasedSource | `2` | DAO tabanlı kaynak |
| FileBasedDataBaseSource | `3` | Dosya tabanlı veritabanı kaynağı |
| WebQuery | `4` | Web sorgusu |
| OLEDBBasedSource | `5` | OLE DB tabanlı kaynak |
| TextBasedSource | `6` | Metin tabanlı kaynak |
| ADORecordSet | `7` | ADO kayıt kümesi |
| DSP | `8` | DSP |
| OLEDBDataModel | `100` | Spreadsheet Data Model tarafından oluşturulan OLE DB veri kaynağı. |
| DataFeedDataModel | `101` | Spreadsheet Data Model tarafından oluşturulan veri akışı veri kaynağı. |
| WorksheetDataModel | `102` | Spreadsheet Data Model tarafından oluşturulan çalışma sayfası veri kaynağı. |
| Table | `102` | Spreadsheet Data Model tarafından oluşturulan çalışma sayfası veri kaynağı. |
| TextDataModel | `103` | Spreadsheet Data Model tarafından oluşturulan metin veri kaynağı. |
| Unknown | `255` | Spreadsheet Data Model tarafından oluşturulan metin veri kaynağı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassConnectionDataSourceTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına örnek veri ekle
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(2000);

            // Çalışma sayfası verilerini kullanarak bir pivot tablo oluştur
            var pivotTable = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            
            // Bağlantıyı al ve ConnectionDataSourceType'ı göster
            var conn = sheet.PivotTables[0].GetSourceDataConnections()[0];
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Class Type: " + conn.ClassType);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


