---
title: "OleObjectCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método OleObjectCollection. Elimina el elemento en el índice especificado"
type: docs
url: /es/net/aspose.cells.drawing/oleobjectcollection/removeat/
---
## OleObjectCollection.RemoveAt method

Elimina el elemento en el índice especificado.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice especificado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar objetos OLE de muestra (3 objetos)
            for (int i = 0; i < 3; i++)
            {
                sheet.OleObjects.Add(i * 10, i * 10, 100, 100, new byte[0]);
            }

            Console.WriteLine("Before removal - OLE Objects count: " + sheet.OleObjects.Count);
            
            // Eliminar objetos OLE uno a uno usando RemoveAt(int index)
            for (int i = sheet.OleObjects.Count - 1; i >= 0; i--)
            {
                sheet.OleObjects.RemoveAt(i);
            }

            Console.WriteLine("After removal - OLE Objects count: " + sheet.OleObjects.Count);
        }
    }
}
```

### Ver también

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


