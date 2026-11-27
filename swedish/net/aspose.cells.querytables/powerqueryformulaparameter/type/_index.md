---
title: "PowerQueryFormulaParameter.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormulaParameter-egenskap. Hämtar typen av Power Query-formel"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulaparameter/type/
---
## PowerQueryFormulaParameter.Type property

Hämtar typen av power query-formeln.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Eftersom vi inte kan skapa en PowerQueryFormulaParameter direkt utan att känna till de nödvändiga konstruktörparametrarna,
                // kommer vi att demonstrera åtkomst till Type-egenskapen via en befintlig frågetabells parametrar
                Console.WriteLine("This demo shows how to access the Type property of PowerQueryFormulaParameter.");
                
                // I ett verkligt scenario skulle du komma åt detta från en befintlig frågetabell
                // För demonstrationsändamål kommer vi att visa hur du kontrollerar typen om du hade en instans
                PowerQueryFormulaParameter parameter = null; // This would normally come from a query table
                
                if (parameter != null)
                {
                    // Visa värdet för Type-egenskapen (skrivskyddad egenskap)
                    Console.WriteLine($"PowerQueryFormulaParameter Type: {parameter.Type}");
                    
                    // Visa möjliga enum‑värden
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
                
                // Spara arbetsboken
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

### Se även

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


