---
title: "OdsPageBackground.IsLink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsPageBackground. Indica si es un gráfico vinculado"
type: docs
url: /es/net/aspose.cells.ods/odspagebackground/islink/
---
## OdsPageBackground.IsLink property

Indica si es un gráfico vinculado.

```csharp
public bool IsLink { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook(FileFormatType.Ods);
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a OdsPageBackground
            OdsPageBackground background = worksheet.PageSetup.ODSPageBackground;

            // Mostrar el valor actual de IsLink
            Console.WriteLine("Current IsLink value: " + background.IsLink);

            // Modificar las propiedades de fondo existentes en lugar de crear una nueva
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Position;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            background.LinkedGraphic = "path/to/image.png";

            // Mostrar el nuevo valor de IsLink
            Console.WriteLine("New IsLink value: " + worksheet.PageSetup.ODSPageBackground.IsLink);

            // Guardar el resultado
            workbook.Save("OdsPageBackgroundIsLinkDemo.ods");
        }
    }
}
```

### Ver también

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


