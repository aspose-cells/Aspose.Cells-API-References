---
title: "WorksheetCollection.Names"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Obtiene la colección de todos los objetos Name en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

Obtiene la colección de todos los objetos Name en la hoja de cálculo.

```csharp
public NameCollection Names { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyNamesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo con caracteres especiales en el nombre
            Worksheet worksheet = workbook.Worksheets.Add("My.Test");
            
            // Acceder a la colección Names
            NameCollection names = workbook.Worksheets.Names;
            
            // Agregar un nuevo rango con nombre
            int index = names.Add("My.Test!TestName");
            Name namedRange = names[index];
            
            // Establecer la referencia del rango y demostrar su uso
            namedRange.RefersTo = "=My.Test!$A$1:$B$2";
            
            // Mostrar las propiedades del rango con nombre
            Console.WriteLine("Name: " + namedRange.Text);
            Console.WriteLine("FullText: " + namedRange.FullText);
            Console.WriteLine("RefersTo: " + namedRange.RefersTo);
        }
    }
}
```

### Ver también

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


