---
title: "ProtectedRangeCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ProtectedRangeCollection. Añade un elemento ProtectedRange a la colección"
type: docs
url: /es/net/aspose.cells/protectedrangecollection/add/
---
## ProtectedRangeCollection.Add method

Añade un elemento [`ProtectedRange`](../../protectedrange/) a la colección.

```csharp
public int Add(string name, int startRow, int startColumn, int endRow, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | Título del rango. Se utiliza como descriptor, no como una definición de rango con nombre. |
| startRow | Int32 | Índice de fila inicial del rango. |
| startColumn | Int32 | Índice de columna inicial del rango. |
| endRow | Int32 | Índice de fila final del rango. |
| endColumn | Int32 | Índice de columna final del rango. |

### Valor de retorno

índice del objeto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionMethodAddWithStringInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
            
            // Añadir rango protegido con nombre y coordenadas
            int index = pranges.Add("Range1", 0, 0, 10, 10);
            
            // Acceder al rango añadido
            ProtectedRange range = pranges[index];
            
            // Establecer descriptor de seguridad
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            range.SecurityDescriptor = securityDescriptor;
            
            // Guardar y verificar
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


