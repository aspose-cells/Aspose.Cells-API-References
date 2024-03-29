---
title: ExternalLinkCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa la colección de enlaces externos en un libro de trabajo.
type: docs
weight: 3370
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
| [Count](../../aspose.cells/externallinkcollection/count) { get; } | Obtiene el número de elementos realmente contenidos en la colección. |
| [Item](../../aspose.cells/externallinkcollection/item) { get; } | Obtiene el[`ExternalLink`](../externallink) elemento en el índice especificado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add#add_1)(string, string[]) | Agrega un enlace externo. |
| [Add](../../aspose.cells/externallinkcollection/add#add)(DirectoryType, string, string[]) | Agregar un enlace externo . |
| [Clear](../../aspose.cells/externallinkcollection/clear#clear)() | Elimina todos los enlaces externos. |
| [Clear](../../aspose.cells/externallinkcollection/clear#clear_1)(bool) | Elimina todos los enlaces externos. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator)() | Obtener un enumerador que itere a través de esta colección. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat#removeat)(int) | Elimina el enlace externo especificado del libro de trabajo. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat#removeat_1)(int, bool) | Elimina el enlace externo especificado del libro de trabajo. |

### Ejemplos

```csharp
[C#]
//Abrir un archivo con enlaces externos
Workbook workbook = new Workbook("book1.xls");

//Cambiar la fuente de datos del enlace externo
workbook.Worksheets.ExternalLinks[0].DataSource = "d:\\link.xls";


[Visual Basic]
'Abrir un archivo con enlaces externos
Dim workbook As Workbook =  New Workbook("book1.xls")

'Cambiar la fuente de datos del enlace externo
workbook.Worksheets.ExternalLinks(0).DataSource = "d:\\link.xls"
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
