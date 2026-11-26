---
title: "Cells.IsDefaultRowHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Indica si la fila está oculta por defecto"
type: docs
url: /es/net/aspose.cells/cells/isdefaultrowhidden/
---
## Cells.IsDefaultRowHidden property

Indica si la fila está oculta por defecto.

```csharp
public bool IsDefaultRowHidden { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHiddenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la propiedad oculta de fila predeterminada
            worksheet.Cells.IsDefaultRowHidden = true;
            
            // Mostrar el valor actual de IsDefaultRowHidden
            Console.WriteLine("IsDefaultRowHidden: " + worksheet.Cells.IsDefaultRowHidden);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


