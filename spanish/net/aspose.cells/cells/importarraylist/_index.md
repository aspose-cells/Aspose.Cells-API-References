---
title: "Cells.ImportArrayList"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Importa una ArrayList de datos en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/importarraylist/
---
## Cells.ImportArrayList method

Importa una arraylist de datos a una hoja de cálculo.

```csharp
public void ImportArrayList(ArrayList arrayList, int firstRow, int firstColumn, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayList | ArrayList | ArrayList de datos. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| isVertical | Booleano | Especifica si se importan los datos verticalmente u horizontalmente. |

### Ejemplos

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportArrayListWithArrayListInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ArrayList data = new ArrayList();
            data.Add("Name");
            data.Add("Age");
            data.Add("City");
            
            cells.ImportArrayList(data, 0, 0, false);
            
            data.Clear();
            data.Add("John");
            data.Add(30);
            data.Add("New York");
            
            cells.ImportArrayList(data, 1, 0, false);
            
            workbook.Save("ImportArrayListDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


