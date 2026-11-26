---
title: "Clase ExternalLinkCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ExternalLinkCollection. Representa la colección de enlaces externos en un libro de trabajo"
type: docs
url: /es/net/aspose.cells/externallinkcollection/
---
## ExternalLinkCollection class

Representa la colección de enlaces externos en un libro de trabajo.

```csharp
public class ExternalLinkCollection : IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count/) { get; } | Obtiene el número de elementos realmente contenidos en la colección. |
| [Item](../../aspose.cells/externallinkcollection/item/) { get; } | Obtiene el elemento [`ExternalLink`](../externallink/) en el índice especificado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add/#add_1)(string, string[]) | Agrega un enlace externo. |
| [Add](../../aspose.cells/externallinkcollection/add/#add)(DirectoryType, string, string[]) | Agregar un enlace externo . |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear)() | Elimina todos los enlaces externos. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear_1)(bool) | Elimina todos los enlaces externos. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator/)() | Obtener un enumerador que recorra esta colección. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat)(int) | Elimina el enlace externo especificado del libro de trabajo. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat_1)(int, bool) | Elimina el enlace externo especificado del libro de trabajo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionDemo
    {
        public static void ExternalLinkCollectionExample()
        {
            // Abrir un archivo con enlaces externos
            Workbook workbook = new Workbook("ExternalLinkCollectionExample_original.xlsx");

            // Obtener la colección de enlaces externos
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;

            // Mostrar el recuento de enlaces externos
            Console.WriteLine("Number of external links: " + externalLinks.Count);

            // Recorrer los enlaces externos y mostrar sus fuentes de datos
            for (int i = 0; i < externalLinks.Count; i++)
            {
                ExternalLink link = externalLinks[i];
                Console.WriteLine("External Link " + i + " Data Source: " + link.DataSource);
            }

            // Agregar un nuevo enlace externo
            int newLinkIndex = externalLinks.Add("newLink.xls", new[] { "Sheet1" });
            Console.WriteLine("Added new external link at index: " + newLinkIndex);

            // Cambiar la fuente de datos del primer enlace externo
            if (externalLinks.Count > 0)
            {
                externalLinks[0].DataSource = "d:\\link.xlsx";
                Console.WriteLine("Updated data source of the first external link.");
            }

            // Guarda el libro de trabajo
            workbook.Save("ExternalLinkCollectionExample.xlsx");

            // Borrar todos los enlaces externos
            externalLinks.Clear();
            Console.WriteLine("Cleared all external links.");

            // Guardar el libro de trabajo después de eliminar los enlaces externos
            workbook.Save("ExternalLinkCollectionExample2.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


