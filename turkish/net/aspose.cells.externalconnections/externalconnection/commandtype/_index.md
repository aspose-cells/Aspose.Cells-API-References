---
title: "ExternalConnection.CommandType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. OLE DB komut tipini belirtir. 1. Sorgu bir küp adını belirtir 2. Sorgu bir SQL ifadesini belirtir 3. Sorgu bir tablo adını belirtir 4. Sorgu varsayılan bilgilerin verildiğini ve yorumlamanın sağlayıcıya bırakıldığını belirtir 5. Sorgu web tabanlı Liste Veri Sağlayıcısına yöneliktir"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/commandtype/
---
## ExternalConnection.CommandType property

OLE DB komut türünü belirtir. 1. Sorgu bir küp adını belirtir 2. Sorgu bir SQL ifadesi belirtir 3. Sorgu bir tablo adını belirtir 4. Sorgu varsayılan bilgilerin verildiğini belirtir ve yorumlama sağlayıcıya bırakılır 5. Sorgu web tabanlı List Data Provider'a yöneliktir.

```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);

            // Bir pivot tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];

            // Harici bağlantıyı al
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // CommandType özelliğini göster
            Console.WriteLine("Original CommandType: " + conn.CommandType);
            
            // CommandType'ı değiştir ve göster
            conn.CommandType = Aspose.Cells.ExternalConnections.OLEDBCommandType.TableName;
            Console.WriteLine("Modified CommandType: " + conn.CommandType);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ExternalConnectionCommandTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


