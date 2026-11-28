---
title: "Sınıf ConnectionParameter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.ConnectionParameter sınıfı. Dış veri bağlantılarıyla kullanılan parametreler hakkında özellikleri belirtir. Parametreler ODBC ve web sorguları için geçerlidir."
type: docs
url: /tr/net/aspose.cells.externalconnections/connectionparameter/
---
## ConnectionParameter class

Harici veri bağlantılarıyla kullanılan parametrelerle ilgili özellikleri belirtir; parametreler ODBC ve web sorguları için geçerlidir.

```csharp
public class ConnectionParameter
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CellReference](../../aspose.cells.externalconnections/connectionparameter/cellreference/) { get; set; } | Sorgu parametresi için hangi hücrenin değerinin kullanılacağını belirten hücre referansı. Yalnızca parameterType hücre olduğunda kullanılır. |
| [Name](../../aspose.cells.externalconnections/connectionparameter/name/) { get; set; } | Parametrenin adı. |
| [Prompt](../../aspose.cells.externalconnections/connectionparameter/prompt/) { get; set; } | Parametre için istem dizesi. Dış veriyi yenilemeden önce parametre değerini toplamak için giriş UI'siyle birlikte elektronik tablo kullanıcısına sunulur. Yalnızca parameterType = prompt olduğunda kullanılır. |
| [RefreshOnChange](../../aspose.cells.externalconnections/connectionparameter/refreshonchange/) { get; set; } | Sorgunun, parametre değerini sağlayan hücrenin içeriği değiştiğinde otomatik olarak yenilenip yenilenmeyeceğini belirten işaret. Doğru ise, dış veri her değişiklikte yeni parametre değeri kullanılarak yenilenir. Yanlış ise, dış veri yalnızca kullanıcı tarafından istendiğinde veya başka bir olay yenilemeyi tetiklediğinde (ör. çalışma kitabı açıldığında) yenilenir. |
| [SqlType](../../aspose.cells.externalconnections/connectionparameter/sqltype/) { get; set; } | Parametrenin SQL veri tipi. Yalnızca ODBC kaynakları için geçerlidir. |
| [Type](../../aspose.cells.externalconnections/connectionparameter/type/) { get; set; } | Kullanılan parametre türü. parameterType=value ise, boolean, double, integer veya string değerlerinden biri kullanılacaktır. Bu durumda, yalnızca {boolean, double, integer veya string} öğelerinden birinin belirtilmesi beklenir. |
| [Value](../../aspose.cells.externalconnections/connectionparameter/value/) { get; set; } | Sorgu parametresi olarak kullanılacak tamsayı olmayan sayısal değer, tamsayı değeri, string değeri veya Boolean değeri. Yalnızca parameterType value olduğunda kullanılır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Yapıcı (constructor) public olmadığı için yansıma (reflection) kullanarak bir bağlantı parametresi oluştur.
                ConnectionParameter parameter = (ConnectionParameter)Activator.CreateInstance(typeof(ConnectionParameter), nonPublic: true);
                
                // Temel özellikleri ayarlayın
                parameter.Name = "CustomerID";
                parameter.Type = ConnectionParameterType.Value;
                parameter.Value = "CUST1001";
                parameter.RefreshOnChange = true;
                parameter.Prompt = "Enter Customer ID:";
                
                // Parametre bilgilerini göster
                Console.WriteLine($"Created parameter: {parameter.Name}");
                Console.WriteLine($"Type: {parameter.Type}");
                Console.WriteLine($"Value: {parameter.Value}");
                Console.WriteLine($"Refresh on change: {parameter.RefreshOnChange}");
                Console.WriteLine($"Prompt: {parameter.Prompt}");
                
                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionParameterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameter: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


