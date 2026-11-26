---
title: "BuiltInDocumentPropertyCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Devuelve un objeto DocumentProperty por el nombre de la propiedad"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

Devuelve un objeto [`DocumentProperty`](../../documentproperty/) por el nombre de la propiedad.

```csharp
public override DocumentProperty this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre de la propiedad sin distinción de mayúsculas a recuperar. |

### Observaciones

Los nombres de cadena de las propiedades corresponden a los nombres de las propiedades tipadas disponibles en [`BuiltInDocumentPropertyCollection`](../).

Si solicita una propiedad que no está presente en el documento, pero el nombre de la propiedad se reconoce como un nombre incorporado válido, se crea una nueva [`DocumentProperty`](../../documentproperty/), se agrega a la colección y se devuelve. La propiedad recién creada se asigna con un valor predeterminado (cadena vacía, cero, falso o DateTime.MinValue según el tipo de la propiedad incorporada).

Si solicita una propiedad que no está presente en el documento y el nombre no se reconoce como un nombre incorporado, se devuelve null.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establezca una propiedad de documento incorporada usando el método adecuado
            workbook.BuiltInDocumentProperties["Version"].Value = "15.0300";
            
            // Acceda e imprima el valor de la propiedad
            Console.WriteLine("Version: " + workbook.BuiltInDocumentProperties["Version"].Value);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Cargue el libro de trabajo guardado y verifique la propiedad
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Version: " + loadedWorkbook.BuiltInDocumentProperties["Version"].Value);
        }
    }
}
```

### Ver también

* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


