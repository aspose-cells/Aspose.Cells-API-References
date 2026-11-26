---
title: "WorksheetCollection.OleSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Obtiene y establece el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole"
type: docs
url: /es/net/aspose.cells/worksheetcollection/olesize/
---
## WorksheetCollection.OleSize property

Obtiene y establece el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole.

```csharp
public object OleSize { get; set; }
```

### Observaciones

Null significa que no hay configuración de tamaño ole.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyOleSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer el tamaño OLE para la colección de hojas de cálculo
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Acceder y mostrar las propiedades del tamaño OLE
            CellArea oleSize = (CellArea)workbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size Range:");
            Console.WriteLine($"StartRow: {oleSize.StartRow}, EndRow: {oleSize.EndRow}");
            Console.WriteLine($"StartColumn: {oleSize.StartColumn}, EndColumn: {oleSize.EndColumn}");
            
            // Guarda el libro de trabajo
            workbook.Save("OleSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


