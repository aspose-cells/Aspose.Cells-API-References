---
title: "DocumentPropertyCollection.Contains"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DocumentPropertyCollection. Devuelve true si una propiedad con el nombre especificado existe en la colección"
type: docs
url: /es/net/aspose.cells.properties/documentpropertycollection/contains/
---
## DocumentPropertyCollection.Contains method

Devuelve true si una propiedad con el nombre especificado existe en la colección.

```csharp
public bool Contains(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad sin distinción de mayúsculas. |

### Valor de retorno

True si la propiedad existe en la colección; false en caso contrario.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodContainsWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Verificar si la propiedad "RevisionNumber" existe en las propiedades de documento incorporadas
            bool containsRevision = workbook.BuiltInDocumentProperties.Contains("RevisionNumber");
            Console.WriteLine("Contains 'RevisionNumber': " + containsRevision);
            
            // Agregar una propiedad personalizada y verificar su existencia
            workbook.CustomDocumentProperties.Add("CustomProperty", "Test Value");
            bool containsCustom = workbook.CustomDocumentProperties.Contains("CustomProperty");
            Console.WriteLine("Contains 'CustomProperty': " + containsCustom);
        }
    }
}
```

### Ver también

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


