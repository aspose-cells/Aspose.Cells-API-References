---
title: "PaneCollection.AcitvePaneType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaneCollection. Obtiene y establece el panel activo"
type: docs
url: /es/net/aspose.cells/panecollection/acitvepanetype/
---
## PaneCollection.AcitvePaneType property

Obtiene y establece el panel activo.

```csharp
[Obsolete("Use PaneCollection.ActivePaneType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public RectangleAlignmentType AcitvePaneType { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad [`ActivePaneType`](../activepanetype/). Este método será eliminado 12 meses después de julio de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PaneCollectionPropertyAcitvePaneTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para demostrar la división de paneles
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i + 1}, Col {j + 1}";
                }
            }

            // Dividir la hoja de cálculo en paneles
            worksheet.Split();

            // Obtener la colección de paneles
            PaneCollection panes = worksheet.GetPanes();

            // Mostrar el panel activo actual
            Console.WriteLine("Current ActivePaneType: " + panes.AcitvePaneType);

            // Establecer el panel activo a BottomRight
            panes.AcitvePaneType = RectangleAlignmentType.BottomRight;
            Console.WriteLine("Changed ActivePaneType to: " + panes.AcitvePaneType);

            // Establecer la primera fila/columna visible para los paneles inferior/derecho
            panes.FirstVisibleRowOfBottomPane = 15;
            panes.FirstVisibleColumnOfRightPane = 7;

            // Guarda el libro de trabajo
            workbook.Save("PaneCollectionActivePaneTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [RectangleAlignmentType](../../../aspose.cells.drawing/rectanglealignmenttype/)
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


