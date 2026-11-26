---
title: "PaneCollection.FirstVisibleColumnOfRightPane"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaneCollection. Obtiene y establece la primera columna visible del panel derecho"
type: docs
url: /es/net/aspose.cells/panecollection/firstvisiblecolumnofrightpane/
---
## PaneCollection.FirstVisibleColumnOfRightPane property

Obtiene y establece la primera columna visible del panel derecho.

```csharp
public int FirstVisibleColumnOfRightPane { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleColumnOfRightPaneDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Congelar paneles especificando los índices de fila y columna (5, 3)
            sheet.FreezePanes(5, 3, 5, 3);
            
            // Obtener la colección de paneles
            PaneCollection panes = sheet.GetPanes();
            
            // Establecer la primera columna visible del panel derecho
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


