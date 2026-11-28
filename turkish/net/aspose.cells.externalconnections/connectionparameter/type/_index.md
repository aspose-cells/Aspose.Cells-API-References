---
title: "ConnectionParameter.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConnectionParameter özelliği. Kullanılan parametrenin türü. Eğer parameterTypevalue ise, boolean, double, integer veya string değerlerinden biri kullanılacaktır. Bu durumda yalnızca boolean, double, integer veya string tiplerinden birinin belirtilmesi beklenir."
type: docs
url: /tr/net/aspose.cells.externalconnections/connectionparameter/type/
---
## ConnectionParameter.Type property

Kullanılan parametre türü. parameterType=value ise, boolean, double, integer veya string değerlerinden biri kullanılacaktır. Bu durumda, yalnızca {boolean, double, integer veya string} öğelerinden birinin belirtilmesi beklenir.

```csharp
public ConnectionParameterType Type { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyTypeDemo
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
                
                // Demonstrasyon amacıyla, bir parametremiz olsaydı Type'ın nasıl kullanılacağını göstereceğiz
                if (parameter != null)
                {
                    // Mevcut Type değerini alın ve görüntüleyin
                    Console.WriteLine("Current Type: " + parameter.Type);
                    
                    // Yeni bir Type değeri ayarlayın (özellik okuma-yazma olduğu için)
                    parameter.Type = ConnectionParameterType.Value;
                    Console.WriteLine("Updated Type: " + parameter.Type);
                }
                else
                {
                    // Parametreyi oluşturamadığımızda yedek bir gösterim
                    workbook.Worksheets[0].Cells["A1"].Value = "Type property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionParameterTypeDemo.xlsx");
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

* enum [ConnectionParameterType](../../connectionparametertype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


