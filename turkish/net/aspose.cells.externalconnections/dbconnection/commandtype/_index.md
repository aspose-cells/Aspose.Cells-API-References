---
title: "DBConnection.CommandType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DBConnection özelliği. OLE DB komut tipini belirtir. 1. Sorgu bir küp adını belirtir 2. Sorgu bir SQL ifadesini belirtir 3. Sorgu bir tablo adını belirtir 4. Sorgu varsayılan bilgilerin verildiğini ve yorumlamanın sağlayıcıya bırakıldığını belirtir 5. Sorgu web tabanlı bir Liste Veri Sağlayıcısına yöneliktir"
type: docs
url: /tr/net/aspose.cells.externalconnections/dbconnection/commandtype/
---
## DBConnection.CommandType property

OLE DB komut türünü belirtir. 1. Sorgu bir küp adını belirtir 2. Sorgu bir SQL ifadesi belirtir 3. Sorgu bir tablo adını belirtir 4. Sorgu varsayılan bilgilerin verildiğini belirtir ve yorumlama sağlayıcıya bırakılır 5. Sorgu web tabanlı List Data Provider'a yöneliktir.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;

    public class DBConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı başlat (boş veya bağlantılar içerebilecek bir dosyadan)
            Workbook workbook = new Workbook();

            try
            {
                // Harici bağlantıların koleksiyonuna erişin
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Koleksiyondaki ilk DBConnection'ı bulun (varsa)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // Geçerli CommandType değerini göster
                    Console.WriteLine("Original CommandType: " + dbConn.CommandType);

                    // CommandType ayarlamayı göster (okuma‑yazma özelliği)
                    dbConn.CommandType = OLEDBCommandType.SqlStatement;
                    Console.WriteLine("Updated CommandType: " + dbConn.CommandType);
                }

                // Çalışma kitabını (değişmemiş olsa bile) kaydet, tam bir akışı göstermek için
                workbook.Save("CommandTypeDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


