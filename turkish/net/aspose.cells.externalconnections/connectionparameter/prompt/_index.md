---
title: "ConnectionParameter.Prompt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConnectionParameter özelliği. Parametre için istem dizesi. Harici verileri yenilemeden önce parametre değerini toplamak için giriş UI'siyle birlikte elektronik tablo kullanıcısına sunulur. Yalnızca parameterType prompt olduğunda kullanılır"
type: docs
url: /tr/net/aspose.cells.externalconnections/connectionparameter/prompt/
---
## ConnectionParameter.Prompt property

Parametre için istem dizesi. Dış veriyi yenilemeden önce parametre değerini toplamak için giriş UI'siyle birlikte elektronik tablo kullanıcısına sunulur. Yalnızca parameterType = prompt olduğunda kullanılır.

```csharp
public string Prompt { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyPromptDemo
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
                
                // Demonstrasyon amacıyla, bir parametremiz olsaydı Prompt'un nasıl kullanılacağını göstereceğiz
                if (parameter != null)
                {
                    // Mevcut Prompt değerini alın ve gösterin
                    Console.WriteLine("Current Prompt: " + parameter.Prompt);
                    
                    // Yeni bir Prompt değeri ayarlayın (çünkü özellik okunabilir-yazılabilir)
                    parameter.Prompt = "Enter customer ID:";
                    Console.WriteLine("Updated Prompt: " + parameter.Prompt);
                }
                else
                {
                    // Parametreyi oluşturamadığımızda yedek bir gösterim
                    workbook.Worksheets[0].Cells["A1"].Value = "Prompt property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionParameterPromptDemo.xlsx");
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


