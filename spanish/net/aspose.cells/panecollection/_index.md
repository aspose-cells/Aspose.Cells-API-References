---
title: "Clase PaneCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.PaneCollection. Representa todos los objetos Pane mostrados en la ventana especificada"
type: docs
url: /es/net/aspose.cells/panecollection/
---
## PaneCollection class

Representa todos los objetos Pane mostrados en la ventana especificada.

```csharp
public class PaneCollection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AcitvePaneType](../../aspose.cells/panecollection/acitvepanetype/) { get; set; } | (**Obsoleto.**) Obtiene y establece el panel activo. |
| [ActivePaneType](../../aspose.cells/panecollection/activepanetype/) { get; set; } | Obtiene y establece el panel activo. |
| [FirstVisibleColumnOfRightPane](../../aspose.cells/panecollection/firstvisiblecolumnofrightpane/) { get; set; } | Obtiene y establece la primera columna visible del panel derecho. |
| [FirstVisibleRowOfBottomPane](../../aspose.cells/panecollection/firstvisiblerowofbottompane/) { get; set; } | Obtiene y establece la primera fila visible del panel inferior. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPaneCollectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].Value = $"Row {i}, Col {j}";
                }
            }
            
            // Congelar paneles en la fila 5, columna 1
            sheet.FreezePanes(5, 1, 5, 1);
            
            // Obtener colección de paneles
            PaneCollection panes = sheet.GetPanes();
            
            // Modificar la configuración de paneles
            panes.FirstVisibleRowOfBottomPane = 5;
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Guarda el libro de trabajo
            workbook.Save("PaneCollectionDemo.xls", SaveFormat.Excel97To2003);
            
            Console.WriteLine("PaneCollection demo executed successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


