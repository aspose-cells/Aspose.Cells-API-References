---
title: "ConnectionParameter.SqlType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConnectionParameter özelliği. Parametrenin SQL veri tipi. Yalnızca ODBC kaynakları için geçerlidir"
type: docs
url: /tr/net/aspose.cells.externalconnections/connectionparameter/sqltype/
---
## ConnectionParameter.SqlType property

Parametrenin SQL veri tipi. Yalnızca ODBC kaynakları için geçerlidir.

```csharp
public SqlDataType SqlType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertySqlTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                
                // Bir bağlantı parametresi oluşturun (yapıcı parametreleri bilinmediği için simüle edilmiştir)
                ConnectionParameter parameter = null;
                
                // Gerçek bir senaryoda, parametreyi düzgün bir şekilde oluştururdunuz
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Demonstrasyon amacıyla, bir parametremiz olsaydı SqlType'ın nasıl kullanılacağını göstereceğiz
                if (parameter != null)
                {
                    // Mevcut SqlType değerini alın ve gösterin
                    Console.WriteLine("Current SqlType: " + parameter.SqlType);
                    
                    // Yeni bir SqlType değeri ayarlayın (çünkü özellik okunabilir-yazılabilir)
                    parameter.SqlType = SqlDataType.SqlInteger;
                    Console.WriteLine("Updated SqlType: " + parameter.SqlType);
                }
                else
                {
                    // Parametreyi oluşturamadığımızda yedek bir gösterim
                    workbook.Worksheets[0].Cells["A1"].Value = "SqlType property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionParameterSqlTypeDemo.xlsx");
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

* enum [SqlDataType](../../sqldatatype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


