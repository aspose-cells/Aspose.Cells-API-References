---
title: PowerQueryFormulaParameter.Value
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaParameter property. Gets the value of parameter
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaparameter/value/
---
## PowerQueryFormulaParameter.Value property

Gets the value of parameter.

```csharp
public string Value { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Parameter Value: &amp;quot; + para.Value);
public static void Property_Value()
        {
            // Create a new workbook
            Workbook workbook = new Workbook(&quot;PowerQueryFormulaDemo_original.xlsx&quot;);

            // Access the DataMashup property of the workbook
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Access the PowerQueryFormulas property
                PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Access the PowerQueryFormulaParameters property
                PowerQueryFormulaParameterCollection powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Example usage: Iterate through PowerQueryFormulas
                foreach (PowerQueryFormula formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Example usage: Iterate through PowerQueryFormulaParameters
                foreach (PowerQueryFormulaParameter para in powerQueryFormulaParameters)
                {
                    // Display the parameter details
                    Console.WriteLine(&quot;Parameter Name: &quot; + para.Name);
                    Console.WriteLine(&quot;Parameter Value: &quot; + para.Value);

                    Console.WriteLine(&quot;Parameter Definition: &quot; + para.ParameterDefinition);
                }
            }
            

            // Save the workbook
            workbook.Save(&quot;PowerQueryFormulaParameterExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


