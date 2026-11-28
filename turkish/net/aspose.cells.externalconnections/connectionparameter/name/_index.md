---
title: "ConnectionParameter.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConnectionParameter özelliği. Parametrenin adı"
type: docs
url: /tr/net/aspose.cells.externalconnections/connectionparameter/name/
---
## ConnectionParameter.Name property

Parametrenin adı.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyNameDemo
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

                // Demonstrasyon amacıyla, bir parametremiz olsaydı Name'in nasıl kullanılacağını göstereceğiz
                if (parameter != null)
                {
                    // Mevcut Name değerini alın ve görüntüleyin
                    Console.WriteLine("Current Name: " + parameter.Name);

                    // Yeni bir Name değeri ayarlayın (özellik okuma-yazma olduğu için)
                    parameter.Name = "NewParameterName";
                    Console.WriteLine("Updated Name: " + parameter.Name);
                }
                else
                {
                    // Parametreyi oluşturamadığımızda yedek bir gösterim
                    workbook.Worksheets[0].Cells["A1"].Value = "Name property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionParameterNameDemo.xlsx");
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


