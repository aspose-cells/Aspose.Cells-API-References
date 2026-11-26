---
title: "Cells.IsColumnHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Verifica si una columna en el índice dado está oculta"
type: docs
url: /es/net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

Comprueba si una columna en el índice dado está oculta.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | índice de columna |

### Valor de retorno

true si la columna está oculta.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsColumnHiddenWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Ocultar la columna C (índice 2)
            cells.HideColumn(2);
            
            // Verificar si la columna C está oculta
            bool isHidden = cells.IsColumnHidden(2);
            
            Console.WriteLine("Is column C (index 2) hidden? " + isHidden);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


