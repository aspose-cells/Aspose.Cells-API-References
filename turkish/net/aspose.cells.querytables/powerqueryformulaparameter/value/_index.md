---
title: "PowerQueryFormulaParameter.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormulaParameter özelliği. Parametrenin değerini alır"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulaparameter/value/
---
## PowerQueryFormulaParameter.Value property

Parametrenin değerini alır.

```csharp
public string Value { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Çalışma kitabının DataMashup özelliğine eriş
                DataMashup dataMashup = workbook.DataMashup;

                if (dataMashup != null)
                {
                    // PowerQueryFormulaParameters koleksiyonuna erişin
                    PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                    // Değer özelliğini göstermek için parametreler arasında yineleme yapın
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Değer özelliğinin mevcut değerini gösterin (okuma işlemi)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Current Value: {parameter.Value}");

                        // Değer okuma/yazma olduğu için yeni bir değer ayarlamayı gösterin
                        string newValue = "UpdatedValue_" + Guid.NewGuid().ToString();
                        parameter.Value = newValue;
                        Console.WriteLine($"Updated Value: {parameter.Value}");
                        Console.WriteLine("----------------------------------------");
                    }

                    if (parameters.Count == 0)
                    {
                        Console.WriteLine("No PowerQueryFormulaParameter instances found in the workbook.");
                    }
                }
                else
                {
                    Console.WriteLine("No DataMashup available in the workbook.");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("ValueDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


