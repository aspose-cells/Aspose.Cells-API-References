---
title: "Style.RotationAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Rappresenta l'angolo di rotazione del testo"
type: docs
url: /it/net/aspose.cells/style/rotationangle/
---
## Style.RotationAngle property

Rappresenta l'angolo di rotazione del testo.

```csharp
public int RotationAngle { get; set; }
```

### Osservazioni

0: Non ruotato.

255: Dall'alto verso il basso.

-90: Downward.

90: Verso l'alto.

Puoi impostare 255 o un valore compreso tra -90 e 90.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile con diversi angoli di rotazione
            Style style1 = workbook.CreateStyle();
            style1.RotationAngle = -90;
            worksheet.Cells["B2"].PutValue("Text rotated -90°");
            worksheet.Cells["B2"].SetStyle(style1);

            Style style2 = workbook.CreateStyle();
            style2.RotationAngle = 90;
            worksheet.Cells["C3"].PutValue("Text rotated 90°");
            worksheet.Cells["C3"].SetStyle(style2);

            Style style3 = workbook.CreateStyle();
            style3.RotationAngle = 255;
            worksheet.Cells["D4"].PutValue("Text rotated 255°");
            worksheet.Cells["D4"].SetStyle(style3);

            // Salva la cartella di lavoro
            workbook.Save("output_rotation_angles.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


