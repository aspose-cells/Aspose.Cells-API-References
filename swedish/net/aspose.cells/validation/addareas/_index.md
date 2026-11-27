---
title: "Validation.AddAreas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsmetod. Tillämpar valideringen på angivna områden"
type: docs
url: /sv/net/aspose.cells/validation/addareas/
---
## Validation.AddAreas method

Tillämpar valideringen på angivna områden.

```csharp
public void AddAreas(CellArea[] areas, bool checkIntersection, bool checkEdge)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| områden | CellArea[] | Områdena. |
| checkIntersection | Boolean | Huruvida man ska kontrollera skärningen av det angivna området med befintliga valideringsområden. Om en validering har tillämpats i det angivna området (eller en del av det), bör den befintliga valideringen först tas bort från det angivna området. Annars kan korruption uppstå för de genererade valideringarna. Om användaren är säker på att alla tillagda områden inte skär någon befintlig area, kan denna parameter sättas till false för prestandaskäl. |
| checkEdge | Boolean | Huruvida man ska kontrollera kanten av denna validerings tillämpade områden. Valideringens interna inställningar beror på det översta vänstra området av dess tillämpade intervall, så om ett av de angivna områdena blir det nya översta vänstra området av de tillämpade intervallen, bör de interna inställningarna ändras och byggas om, annars kan oväntade resultat uppstå. Om användaren är säker på att inget av de tillagda områdena är det översta vänstra, kan denna parameter sättas till false för prestandaskäl. |

### Anmärkningar

I den här metoden kommer vi att ta bort alla gamla valideringar i det angivna området. För det översta vänstra av Valideringens tillämpade intervall är först dess StartRow den minsta, därefter är dess StartColumn den minsta av de områden som har samma minsta StartRow.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodAddAreasWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.List;
            validation.AlertStyle = ValidationAlertType.Stop;
            validation.Operator = OperatorType.None;
            validation.Formula1 = "1,2,3";
            validation.InCellDropDown = true;

            CellArea[] areas = new CellArea[2];
            areas[0] = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 1 };
            areas[1] = new CellArea { StartRow = 2, StartColumn = 2, EndRow = 3, EndColumn = 3 };

            try
            {
                validation.AddAreas(areas, true, false);
                Console.WriteLine("Added validation areas with checkIntersection=true, checkEdge=false");

                foreach (CellArea area in validation.Areas)
                {
                    Console.WriteLine($"Validation area: R{area.StartRow + 1}C{area.StartColumn + 1}:R{area.EndRow + 1}C{area.EndColumn + 1}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding validation areas: {ex.Message}");
            }

            workbook.Save("ValidationAddAreasDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


