---
title: "PowerQueryFormulaParameter.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormulaParameter özelliği. Power query formülünün tipini alır"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulaparameter/type/
---
## PowerQueryFormulaParameter.Type property

Power query formülünün tipini alır.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Gerekli yapıcı parametrelerini bilmeden PowerQueryFormulaParameter'ı doğrudan oluşturamadığımız için,
                // Mevcut bir sorgu tablosunun parametreleri aracılığıyla Type özelliğine erişimi göstereceğiz
                Console.WriteLine("This demo shows how to access the Type property of PowerQueryFormulaParameter.");
                
                // Gerçek bir senaryoda, bunu mevcut bir sorgu tablosundan erişirdiniz
                // Demonstrasyon amaçlı, bir örnek varsa tipin nasıl kontrol edileceğini göstereceğiz
                PowerQueryFormulaParameter parameter = null; // This would normally come from a query table
                
                if (parameter != null)
                {
                    // Type özelliğinin değerini gösterin (yalnızca okuma özelliği)
                    Console.WriteLine($"PowerQueryFormulaParameter Type: {parameter.Type}");
                    
                    // Olası enum değerlerini göster
                    Console.WriteLine("Possible PowerQueryFormulaType values:");
                    foreach (PowerQueryFormulaType type in Enum.GetValues(typeof(PowerQueryFormulaType)))
                    {
                        Console.WriteLine($"- {type}");
                    }
                }
                else
                {
                    Console.WriteLine("No PowerQueryFormulaParameter instance available for demonstration.");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("TypeDemo.xlsx");
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

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


