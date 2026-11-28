---
title: "PowerQueryFormulaParameter.FormulaDefinition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormulaParameter özelliği. Parametrenin tanımını alır"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/
---
## PowerQueryFormulaParameter.FormulaDefinition property

Parametrenin tanımını alır.

```csharp
public override string FormulaDefinition { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyFormulaDefinitionDemo
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

                    // FormulaDefinition'ı göstermek için parametreler üzerinde yineleme yapın
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // FormulaDefinition özelliğinin değerini göster (yalnızca okuma özelliği)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Formula Definition: {parameter.FormulaDefinition}");
                        Console.WriteLine($"Parameter Value: {parameter.Value}");
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
                workbook.Save("FormulaDefinitionDemo.xlsx");
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


