---
title: "OdsPageBackground.IsLink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsPageBackground. Indica se è una grafica collegata"
type: docs
url: /it/net/aspose.cells.ods/odspagebackground/islink/
---
## OdsPageBackground.IsLink property

Indica se è una grafica collegata.

```csharp
public bool IsLink { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsPageBackgroundPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook(FileFormatType.Ods);
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a OdsPageBackground
            OdsPageBackground background = worksheet.PageSetup.ODSPageBackground;

            // Visualizza il valore corrente di IsLink
            Console.WriteLine("Current IsLink value: " + background.IsLink);

            // Modifica le proprietà di sfondo esistenti invece di crearne una nuova
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Position;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            background.LinkedGraphic = "path/to/image.png";

            // Visualizza il nuovo valore di IsLink
            Console.WriteLine("New IsLink value: " + worksheet.PageSetup.ODSPageBackground.IsLink);

            // Salva il risultato
            workbook.Save("OdsPageBackgroundIsLinkDemo.ods");
        }
    }
}
```

### Vedi anche

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


