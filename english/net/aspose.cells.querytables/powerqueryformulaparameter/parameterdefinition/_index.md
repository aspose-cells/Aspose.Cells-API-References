---
title: PowerQueryFormulaParameter.ParameterDefinition
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaParameter property. Gets the definition of the parameter
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/
---
## PowerQueryFormulaParameter.ParameterDefinition property

Gets the definition of the parameter.

```csharp
[Obsolete("Use PowerQueryFormulaParameter.FormulaDefinition property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ParameterDefinition { get; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use PowerQueryFormulaParameter.FormulaDefinition property. This property will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
public static void Property_ParameterDefinition()
        {
            // Create a new workbook
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

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
                    Console.WriteLine("Parameter Name: " + para.Name);
                    Console.WriteLine("Parameter Value: " + para.Value);

                    Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
                }
            }
            

            // Save the workbook
            workbook.Save("PowerQueryFormulaParameterExample.xlsx");

            return;
        }
```

### See Also

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


