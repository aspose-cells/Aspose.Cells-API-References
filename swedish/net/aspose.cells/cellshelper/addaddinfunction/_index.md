---
title: "CellsHelper.AddAddInFunction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Lägg till tilläggsfunktion"
type: docs
url: /sv/net/aspose.cells/cellshelper/addaddinfunction/
---
## CellsHelper.AddAddInFunction method

Lägg till tilläggsfunktion.

```csharp
[Obsolete("Use WorksheetCollection.RegisterAddInFunction() methods instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static void AddAddInFunction(string function, int minCountOfParameters, 
    int maxCountOfParameters, ParameterType[] paramersType, ParameterType functionValueType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| funktion | String | Funktionens namn. |
| minCountOfParameters | Int32 | Minsta antal parametrar som den här funktionen kräver |
| maxCountOfParameters | Int32 | Maximalt antal parametrar som den här funktionen tillåter. |
| paramersType | ParameterType[] | Den förväntade parametertypen för funktionen |
| functionValueType | ParameterType | Funktionens värdetyp. |

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd i stället WorksheetCollection.RegisterAddInFunction() metoderna. Denna metod kommer att tas bort 12 månader senare från och med januari 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodAddAddInFunctionWithStringInt32Int32ParameterTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Definiera parametrar för AddAddInFunction
                string functionName = "CUSTOMFUNCTION";
                int minParams = 2;
                int maxParams = 4;
                ParameterType[] paramTypes = new ParameterType[] { ParameterType.Value, ParameterType.Reference };
                ParameterType returnType = ParameterType.Value;

                // Anropa AddAddInFunction-metoden
                CellsHelper.AddAddInFunction(functionName, minParams, maxParams, paramTypes, returnType);

                // Använd den anpassade funktionen i en cell
                worksheet.Cells["A1"].Formula = "=CUSTOMFUNCTION(5,B2)";
                worksheet.Cells["B2"].Value = 10;

                // Beräkna formler
                workbook.CalculateFormula();

                Console.WriteLine("AddAddInFunction executed successfully. Custom function added and used in A1.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAddInFunction method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("AddAddInFunctionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ParameterType](../../parametertype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


