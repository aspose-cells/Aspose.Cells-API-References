---
title: "PaneCollection.FirstVisibleRowOfBottomPane"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaneCollection. Obtiene y establece la primera fila visible del panel inferior"
type: docs
url: /es/net/aspose.cells/panecollection/firstvisiblerowofbottompane/
---
## PaneCollection.FirstVisibleRowOfBottomPane property

Obtiene y establece la primera fila visible del panel inferior.

```csharp
public int FirstVisibleRowOfBottomPane { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para crear un panel desplazable
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Congelar paneles en la fila 10 (esto creará paneles superior e inferior)
            worksheet.FreezePanes(10, 0, 10, 0);
            
            // Obtener la colección de paneles
            PaneCollection panes = worksheet.GetPanes();
            
            // Establecer la primera fila visible del panel inferior
            panes.FirstVisibleRowOfBottomPane = 15;
            
            // Mostrar la primera fila visible del panel inferior
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            
            // Guarda el libro de trabajo
            workbook.Save("PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


