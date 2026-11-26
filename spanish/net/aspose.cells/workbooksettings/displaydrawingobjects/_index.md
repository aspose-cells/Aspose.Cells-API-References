---
title: "WorkbookSettings.DisplayDrawingObjects"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Indica si y cómo mostrar objetos en el libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/displaydrawingobjects/
---
## WorkbookSettings.DisplayDrawingObjects property

Indica si y cómo mostrar objetos en el libro.

```csharp
public DisplayDrawingObjects DisplayDrawingObjects { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDisplayDrawingObjectsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Agregar una forma de ejemplo para demostrar la propiedad
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Establecer para mostrar todas las formas
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
            workbook.Save("DisplayShapes.xlsx");

            // Establecer para mostrar marcadores de posición
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;
            workbook.Save("Placeholders.xlsx");

            // Establecer para ocultar todas las formas
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;
            workbook.Save("Hide.xlsx");
        }
    }
}
```

### Ver también

* enum [DisplayDrawingObjects](../../displaydrawingobjects/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


