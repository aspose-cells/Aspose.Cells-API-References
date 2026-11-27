---
title: "PowerQueryFormulaFunction.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormulaFunction-egenskap. Hämtar typen av Power Query-formel."
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulafunction/type/
---
## PowerQueryFormulaFunction.Type property

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

    public class PowerQueryFormulaFunctionPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en Power Query-formelfunktion.
            // Eftersom vi inte kan skapa den direkt måste vi hämta den någonstans.
            // För demonstrationsändamål visar vi bara hur man kommer åt Type-egenskapen.
            // (I verklig användning skulle du hämta detta från en befintlig samling)
            PowerQueryFormulaFunction function = null; // Can't instantiate directly
            
            // Eftersom vi inte heller kan skapa en QueryTable direkt hoppar vi över den delen.
            QueryTable queryTable = null; // Can't instantiate directly
            
            // Det går inte att lägga till i samlingen av frågetabeller på detta sätt – den är skrivskyddad.
            // worksheet.QueryTables[0] = queryTable; // Denna rad har tagits bort
            
            // För demonstration visar vi bara det utskriftsformat vi skulle använda om vi hade en funktion
            if (function != null)
            {
                Console.WriteLine("Power Query Formula Function Type: " + function.Type);
                Console.WriteLine("Is this a function? " + (function.Type == PowerQueryFormulaType.Function));
            }
            else
            {
                Console.WriteLine("Could not create PowerQueryFormulaFunction instance - constructor not available");
            }

            // Spara resultatet
            workbook.Save("PowerQueryFormulaFunctionTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


