---
title: "Validation.AddArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsmetod. Tillämpar valideringen på området"
type: docs
url: /sv/net/aspose.cells/validation/addarea/
---
## AddArea(CellArea) {#addarea}

Tillämpar valideringen på området.

```csharp
public void AddArea(CellArea cellArea)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | CellArea | Området. |

### Anmärkningar

Det är ekvivalent att använda `AddArea` med kontroll av intersektion och kant.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Skapa en validering
            ValidationCollection vc = sheet.Validations;
            Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
            validation.Type = ValidationType.List;
            validation.Formula1 = "=A1:A10";

            // Lägg till fler områden till valideringen
            for (int i = 1; i < 5; i++)
            {
                validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
            }

            // Spara arbetsboken
            wb.Save("ValidationMethodAddAreaWithCellAreaDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Validation with multiple areas created successfully.");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddArea(CellArea, bool, bool) {#addarea_1}

Tillämpar valideringen på området.

```csharp
public void AddArea(CellArea cellArea, bool checkIntersection, bool checkEdge)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | CellArea | Området. |
| checkIntersection | Boolean | Om intersektionen av det angivna området med befintliga valideringars områden ska kontrolleras. Om en validering har tillämpats i det angivna området (eller en del av det), bör den befintliga valideringen först tas bort från det angivna området. Annars kan korruption uppstå för de genererade Valideringarna. Om användaren är säker på att det tillagda området inte korsar något befintligt område, kan denna parameter sättas till false av prestandaskäl. |
| checkEdge | Boolean | Om kanten av denna validerings tillämpade områden ska kontrolleras. Valideringens interna inställningar beror på det översta vänstra området av dess tillämpade intervall, så om det angivna området blir det nya översta vänstra intervallet, bör de interna inställningarna ändras och byggas om, annars kan oväntade resultat uppstå. Om användaren är säker på att det tillagda området inte är det översta vänstra, kan denna parameter sättas till false av prestandaskäl. |

### Anmärkningar

I den här metoden kommer vi att ta bort alla gamla valideringar i det angivna området. För det översta vänstra av Valideringens tillämpade intervall är först dess StartRow den minsta, därefter är dess StartColumn den minsta av de områden som har samma minsta StartRow.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en validering i ett specifikt område
            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "F3";

            // Demonstrera AddArea med CellArea och två boolska parametrar
            validation.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
            Console.WriteLine("Area count after AddArea: " + validation.Areas.Length);
            Console.WriteLine("Formula1 after AddArea: " + validation.Formula1);

            // Ta bort det tillagda området
            validation.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
            Console.WriteLine("Area count after RemoveArea: " + validation.Areas.Length);

            // Lägg till flera områden med en bulkoperation
            CellArea[] areas = new CellArea[10];
            for (int i = 0; i < areas.Length; i++)
            {
                areas[i] = CellArea.CreateCellArea(6 + i, 3, 6 + i, 4);
            }
            validation.AddAreas(areas, true, true);
            Console.WriteLine("Area count after bulk AddAreas: " + validation.Areas.Length);

            // Spara arbetsboken
            workbook.Save("ValidationMethodAddAreaDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


