---
title: "WorksheetCollection.SortNames"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Ordena los nombres definidos"
type: docs
url: /es/net/aspose.cells/worksheetcollection/sortnames/
---
## WorksheetCollection.SortNames method

Ordena los nombres definidos.

```csharp
public void SortNames()
```

### Observaciones

Si crea una gran cantidad de rangos con nombre en el archivo Excel, por favor llame a este método después de crear todos los rangos con nombre y antes de guardar

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSortNamesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos rangos con nombre
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test1");
            worksheet.Cells.CreateRange("A1").Name = "Range2";
            worksheet.Cells["B1"].PutValue("Test2");
            worksheet.Cells.CreateRange("B1").Name = "Range1";
            
            // Mostrar nombres antes de ordenar
            Console.WriteLine("Before sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Ordenar los nombres
            workbook.Worksheets.SortNames();
            
            // Mostrar nombres después de ordenar
            Console.WriteLine("\nAfter sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


