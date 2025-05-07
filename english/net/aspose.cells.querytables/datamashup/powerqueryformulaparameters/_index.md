---
title: DataMashup.PowerQueryFormulaParameters
second_title: Aspose.Cells for .NET API Reference
description: DataMashup property. Gets power query formula parameters
type: docs
url: /net/aspose.cells.querytables/datamashup/powerqueryformulaparameters/
---
## DataMashup.PowerQueryFormulaParameters property

Gets power query formula parameters.

```csharp
[Obsolete("Use DataMashup.PowerQueryFormulas property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PowerQueryFormulaParameterCollection PowerQueryFormulaParameters { get; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use DataMashup.PowerQueryFormulas property. This property will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;
public static void Property_PowerQueryFormulaParameters()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the DataMashup property of the workbook
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null )
            {
                // Access the PowerQueryFormulas property
                var powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Access the PowerQueryFormulaParameters property
                var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Example usage: Iterate through PowerQueryFormulas
                foreach (var formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Example usage: Iterate through PowerQueryFormulaParameters
                foreach (var parameter in powerQueryFormulaParameters)
                {
                    Console.WriteLine(parameter.Name);
                }
            }
            

            // Save the workbook
            workbook.Save("DataMashupExample.xlsx");
            workbook.Save("DataMashupExample.pdf");
            return;
        }
```

### See Also

* class [PowerQueryFormulaParameterCollection](../../powerqueryformulaparametercollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


