---
title: "Enum OLEDBCommandType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.OLEDBCommandType enum. OLE DB komut türünü belirtir"
type: docs
url: /tr/net/aspose.cells.externalconnections/oledbcommandtype/
---
## OLEDBCommandType enumeration

OLE DB komut türünü belirtir.

```csharp
public enum OLEDBCommandType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Komut türü belirtilmemiştir. |
| CubeName | `1` | Bir küp adını belirtir |
| SqlStatement | `2` | Bir SQL ifadesini belirtir |
| TableName | `3` | Bir tablo adını belirtir |
| DefaultInformation | `4` | Varsayılan bilginin verildiğini ve yorumlamanın sağlayıcıya bırakıldığını belirtir. |
| WebBasedList | `5` | Web tabanlı Liste Veri Sağlayıcısına karşı bir sorgu olduğunu belirtir. |
| TableCollection | `6` | Tablo listesini belirtir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassOLEDBCommandTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Harici bağlantıyı al
            ExternalConnectionCollection connections = workbook.DataConnections;
            ExternalConnection conn = connections[0];
            
            // OLEDBCommandType kullanımını göster
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command Type: " + conn.CommandType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Komut türünü değiştir ve göster
            conn.CommandType = OLEDBCommandType.TableName;
            Console.WriteLine("\nAfter changing CommandType:");
            Console.WriteLine("Command Type: " + conn.CommandType);
            
            // Çalışma kitabını kaydedin
            workbook.Save("OLEDBCommandTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


