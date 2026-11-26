---
title: "ContentTypeProperty.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ContentTypeProperty. Devuelve o establece el nombre del objeto"
type: docs
url: /es/net/aspose.cells.properties/contenttypeproperty/name/
---
## ContentTypeProperty.Name property

Devuelve o establece el nombre del objeto.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una propiedad de tipo de contenido con el nombre "ss"
            workbook.ContentTypeProperties.Add("ss", "bb", "text");
            
            // Guardar en formato XLS
            workbook.Save("example.xls");
            
            // Recargar el libro de trabajo y verificar la propiedad Name
            workbook = new Workbook("example.xls");
            Console.WriteLine("Name property in XLS: " + workbook.ContentTypeProperties[0].Name);
            
            // Guardar en formato XLSX
            workbook.Save("example.xlsx");
            
            // Recargar y verificar de nuevo
            workbook = new Workbook("example.xlsx");
            Console.WriteLine("Name property in XLSX: " + workbook.ContentTypeProperties[0].Name);
        }
    }
}
```

### Ver también

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


