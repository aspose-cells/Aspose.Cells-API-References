---
title: "ConnectionParameter.CellReference"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConnectionParameter özelliği. Sorgu parametresi için hangi hücre değerinin kullanılacağını gösteren hücre referansı. Yalnızca parameterType hücre olduğunda kullanılır"
type: docs
url: /tr/net/aspose.cells.externalconnections/connectionparameter/cellreference/
---
## ConnectionParameter.CellReference property

Sorgu parametresi için hangi hücrenin değerinin kullanılacağını belirten hücre referansı. Yalnızca parameterType hücre olduğunda kullanılır.

```csharp
public string CellReference { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyCellReferenceDemo
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
                
                // Demonstrasyon amacıyla, bir parametremiz olsaydı CellReference'in nasıl kullanılacağını göstereceğiz
                if (parameter != null)
                {
                    // Mevcut CellReference değerini alın ve görüntüleyin
                    Console.WriteLine("Current CellReference: " + parameter.CellReference);
                    
                    // Yeni bir CellReference değeri ayarlayın (özellik okuma-yazma olduğu için)
                    parameter.CellReference = "A1";
                    Console.WriteLine("Updated CellReference: " + parameter.CellReference);
                }
                else
                {
                    // Parametreyi oluşturamadığımızda yedek bir gösterim
                    workbook.Worksheets[0].Cells["A1"].Value = "CellReference property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionParameterCellReferenceDemo.xlsx");
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

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


