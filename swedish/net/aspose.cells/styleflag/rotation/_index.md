---
title: "StyleFlag.Rotation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag egenskap. Rotationsinställning kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/rotation/
---
## StyleFlag.Rotation property

Rotationsinställning kommer att tillämpas.

```csharp
public bool Rotation { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyRotationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt cell A1 och ange lite text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Rotated Text");

            // Hämta stil för cellen
            Style style = workbook.CreateStyle();

            // Ange nytt rotationsvärde (45 grader)
            style.RotationAngle = 45;

            // Visa aktuellt rotationsvärde
            Console.WriteLine("Current Rotation value: " + cell.GetStyle().RotationAngle);            

            // Skapa en stilflagga och aktivera rotationsflaggan
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Rotation = true;

            // Applicera stilen med rotation på cellen
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("after setting style, rotation value: " + cell.GetStyle().RotationAngle);
           
            // Spara resultatet
            workbook.Save("PropertyRotationDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


