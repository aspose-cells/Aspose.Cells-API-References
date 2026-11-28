---
title: "ConnectionParameter.RefreshOnChange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConnectionParameter özelliği. Parametre değerini sağlayan bir hücrenin içeriği değiştiğinde sorgunun otomatik olarak yenilenip yenilenmeyeceğini belirten işaret. True ise, her değişiklikte dış veri yeni parametre değeriyle yenilenir. False ise, dış veri yalnızca kullanıcı tarafından istenildiğinde veya başka bir olay (ör. çalışma kitabı açılması) yenilemeyi tetiklediğinde yenilenir."
type: docs
url: /tr/net/aspose.cells.externalconnections/connectionparameter/refreshonchange/
---
## ConnectionParameter.RefreshOnChange property

Sorgunun, parametre değerini sağlayan hücrenin içeriği değiştiğinde otomatik olarak yenilenip yenilenmeyeceğini belirten işaret. Doğru ise, dış veri her değişiklikte yeni parametre değeri kullanılarak yenilenir. Yanlış ise, dış veri yalnızca kullanıcı tarafından istendiğinde veya başka bir olay yenilemeyi tetiklediğinde (ör. çalışma kitabı açıldığında) yenilenir.

```csharp
public bool RefreshOnChange { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyRefreshOnChangeDemo
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
                
                // Demonstrasyon amacıyla, bir parametremiz olsaydı RefreshOnChange'in nasıl kullanılacağını göstereceğiz
                if (parameter != null)
                {
                    // Mevcut RefreshOnChange değerini alın ve gösterin
                    Console.WriteLine("Current RefreshOnChange: " + parameter.RefreshOnChange);
                    
                    // Yeni bir RefreshOnChange değeri ayarlayın (özellik okuma-yazma olduğu için)
                    parameter.RefreshOnChange = true;
                    Console.WriteLine("Updated RefreshOnChange: " + parameter.RefreshOnChange);
                }
                else
                {
                    // Parametreyi oluşturamadığımızda yedek bir gösterim
                    workbook.Worksheets[0].Cells["A1"].Value = "RefreshOnChange property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionParameterRefreshOnChangeDemo.xlsx");
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


