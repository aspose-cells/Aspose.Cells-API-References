---
title: "WorksheetCollection.SetOleSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Establece el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole"
type: docs
url: /es/net/aspose.cells/worksheetcollection/setolesize/
---
## WorksheetCollection.SetOleSize method

Establece el tamaño mostrado cuando el archivo Workbook se usa como objeto Ole.

```csharp
public void SetOleSize(int startRow, int endRow, int startColumn, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | Índice de fila inicial. |
| endRow | Int32 | Índice de fila final. |
| startColumn | Int32 | Índice de columna inicial. |
| endColumn | Int32 | Índice de columna final. |

### Observaciones

Este método se usa generalmente para ajustar el tamaño de visualización en archivos ppt o doc.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSetOleSizeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer el tamaño OLE para las hojas de cálculo
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verificar el tamaño OLE
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CellArea oleSize = (CellArea)loadedWorkbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size - StartRow: {0}, EndRow: {1}, StartColumn: {2}, EndColumn: {3}", 
                oleSize.StartRow, oleSize.EndRow, oleSize.StartColumn, oleSize.EndColumn);
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


