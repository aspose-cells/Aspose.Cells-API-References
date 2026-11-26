---
title: "Enumeración DisplayDrawingObjects"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.DisplayDrawingObjects. Representa si y cómo mostrar los objetos en el libro de trabajo"
type: docs
url: /es/net/aspose.cells/displaydrawingobjects/
---
## DisplayDrawingObjects enumeration

Representa si y cómo mostrar objetos en el libro de trabajo.

```csharp
public enum DisplayDrawingObjects
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DisplayShapes | `0` | Mostrar todos los objetos |
| Placeholders | `1` | Mostrar marcadores de posición |
| Hide | `2` | Ocultar todas las formas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DisplayDrawingObjectsDemo
    {
        public static void DisplayDrawingObjectsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establecer la propiedad DisplayDrawingObjects para mostrar todos los objetos
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;

            // Guarda el libro de trabajo
            workbook.Save("DisplayDrawingObjectsExample_DisplayShapes.xlsx");

            // Establecer la propiedad DisplayDrawingObjects para mostrar marcadores de posición
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;

            // Guarda el libro de trabajo
            workbook.Save("DisplayDrawingObjectsExample_Placeholders.xlsx");

            // Establecer la propiedad DisplayDrawingObjects para ocultar todas las formas
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;

            // Guarda el libro de trabajo
            workbook.Save("DisplayDrawingObjectsExample_Hide.xlsx");
            workbook.Save("DisplayDrawingObjectsExample_Hide.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


