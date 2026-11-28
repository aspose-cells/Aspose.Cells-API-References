---
title: "ConnectionParameter.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConnectionParameter özelliği. Sorgu parametresi olarak kullanılacak tam sayı olmayan sayısal değer, tam sayı değeri, metin değeri veya Boolean değeri. Yalnızca parameterType değerinin value olduğu durumlarda kullanılır."
type: docs
url: /tr/net/aspose.cells.externalconnections/connectionparameter/value/
---
## ConnectionParameter.Value property

Sorgu parametresi olarak kullanılacak tamsayı olmayan sayısal değer, tamsayı değeri, string değeri veya Boolean değeri. Yalnızca parameterType value olduğunda kullanılır.

```csharp
public object Value { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                
                // Bir bağlantı parametresi oluşturun (yapıcı parametrelerini bilmediğimiz için simüle edilmiştir)
                ConnectionParameter parameter = null;
                
                // Gerçek bir senaryoda, parametreyi düzgün bir şekilde oluştururdunuz
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Demonstrasyon amacıyla, bir değer içeren sahte bir parametre oluşturacağız
                // Bu, Value özelliğinin pratikte nasıl kullanılacağını gösterir
                if (parameter != null)
                {
                    // Değeri ayarlayın (çünkü Value okunabilir-yazılabilir)
                    parameter.Value = "SampleParameterValue";
                    
                    // Değeri alın ve gösterin
                    Console.WriteLine("Parameter Value: " + parameter.Value);
                    
                    // Değerin değiştirilebilir olduğunu göstermek için değeri değiştirin
                    parameter.Value = 42;
                    Console.WriteLine("Updated Parameter Value: " + parameter.Value);
                }
                else
                {
                    // Parametreyi oluşturamadığımızda yedek bir gösterim
                    workbook.Worksheets[0].Cells["A1"].Value = "Value property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionParameterValueDemo.xlsx");
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


