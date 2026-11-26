---
title: "Worksheet.SetVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Establece las opciones de visibilidad"
type: docs
url: /es/net/aspose.cells/worksheet/setvisible/
---
## Worksheet.SetVisible method

Establece las opciones visibles.

```csharp
public void SetVisible(bool isVisible, bool ignoreError)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isVisible | Booleano | Indica si la hoja de cálculo es visible |
| ignoreError | Booleano | Indica si se debe ignorar el error si esta opción no es válida. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSetVisibleWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunas hojas de cálculo
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Establecer la visibilidad de las hojas de cálculo
            // Primer parámetro: isVisible - false para ocultar la hoja
            // Segundo parámetro: ignoreError - true para ignorar el error si la hoja no se puede ocultar
            workbook.Worksheets["Sheet2"].SetVisible(false, true);
            workbook.Worksheets["Sheet3"].SetVisible(false, true);

            // Guarda el libro de trabajo
            workbook.Save("WorksheetVisibilityDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


