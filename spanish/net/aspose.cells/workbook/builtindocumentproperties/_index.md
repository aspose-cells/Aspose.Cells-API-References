---
title: "Workbook.BuiltInDocumentProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del libro de trabajo. Devuelve una colección DocumentProperty que representa todas las propiedades de documento incorporadas de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/workbook/builtindocumentproperties/
---
## Workbook.BuiltInDocumentProperties property

Devuelve una colección [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento integradas de la hoja de cálculo.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Observaciones

No se puede agregar una nueva propiedad a la lista de propiedades de documento integradas. Solo puedes obtener una propiedad integrada y cambiar su valor. La siguiente es la lista de nombres de propiedades integradas:

Título

Asunto

Autor

Palabras clave

Comentarios

Plantilla

Último autor

Número de revisión

Nombre de la aplicación

Fecha de última impresión

Fecha de creación

Hora de la última guardada

Tiempo total de edición

Número de páginas

Número de palabras

Número de caracteres

Seguridad

Categoría

Formato

Gerente

Empresa

Número de bytes

Número de líneas

Número de párrafos

Número de diapositivas

Número de notas

Número de diapositivas ocultas

Número de clips multimedia

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder y modificar las propiedades de documento incorporadas
            DocumentProperty authorProperty = workbook.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Workbook";
            
            // Mostrar las propiedades modificadas
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties["Title"].Value);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


