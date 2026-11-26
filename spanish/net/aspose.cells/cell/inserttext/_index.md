---
title: "Cell.InsertText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Insertar algunos caracteres en la celda. Si la celda tiene formato enriquecido, este método puede mantener el formato original."
type: docs
url: /es/net/aspose.cells/cell/inserttext/
---
## Cell.InsertText method

Inserta algunos caracteres en la celda. Si la celda tiene formato enriquecido, este método puede conservar el formato original.

```csharp
public void InsertText(int index, string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice. |
| texto | String | Texto insertado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceda a la celda B3 y establezca el valor inicial
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("OriginalText");
            
            // Inserte texto en la posición 6
            cell.InsertText(6, "Inserted");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


