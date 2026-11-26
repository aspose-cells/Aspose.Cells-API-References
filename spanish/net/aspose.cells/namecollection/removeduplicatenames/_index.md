---
title: "NameCollection.RemoveDuplicateNames"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método NameCollection. Eliminar los nombres definidos duplicados"
type: docs
url: /es/net/aspose.cells/namecollection/removeduplicatenames/
---
## NameCollection.RemoveDuplicateNames method

Eliminar los nombres definidos duplicados

```csharp
public void RemoveDuplicateNames()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveDuplicateNamesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos rangos con nombre con nombres duplicados
            worksheet.Cells["A1"].PutValue("Test Value 1");
            worksheet.Cells["B1"].PutValue("Test Value 2");
            
            // Crear rangos con nombre duplicados usando la firma correcta del método Add
            int index1 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$B$1";
            
            // Mostrar recuento antes de eliminar duplicados
            Console.WriteLine($"Named ranges count before removal: {workbook.Worksheets.Names.Count}");
            
            // Eliminar nombres duplicados
            workbook.Worksheets.Names.RemoveDuplicateNames();
            
            // Mostrar recuento después de eliminar duplicados
            Console.WriteLine($"Named ranges count after removal: {workbook.Worksheets.Names.Count}");
        }
    }
}
```

### Ver también

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


