---
title: CustomDocumentPropertyCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Una colección de propiedades de documentos personalizados.
type: docs
weight: 4830
url: /es/net/aspose.cells.properties/customdocumentpropertycollection/
---
## CustomDocumentPropertyCollection class

Una colección de propiedades de documentos personalizados.

```csharp
public class CustomDocumentPropertyCollection : DocumentPropertyCollection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells.properties/documentpropertycollection/count) { get; } | Obtiene el número de elementos de la colección. |
| [Item](../../aspose.cells.properties/documentpropertycollection/item) { get; } | Devuelve un[`DocumentProperty`](../documentproperty)objeto por index. |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item) { get; } | Devuelve un[`DocumentProperty`](../documentproperty) objeto por el nombre de la propiedad. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add#add)(string, bool) | Crea una nueva propiedad de documento personalizada del **PropertyType.Boolean** tipo de datos. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add#add_3)(string, DateTime) | Crea una nueva propiedad de documento personalizada del **PropertyType.DateTime** tipo de datos. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add#add_1)(string, double) | Crea una nueva propiedad de documento personalizada del **PropertyType.Float** tipo de datos. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add#add_2)(string, int) | Crea una nueva propiedad de documento personalizada del **PropertyType.Number** tipo de datos. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add#add_4)(string, string) | Crea una nueva propiedad de documento personalizada del **PropertyType.String** tipo de datos. |
| [AddLinkToContent](../../aspose.cells.properties/customdocumentpropertycollection/addlinktocontent)(string, string) | Crea una nueva propiedad de documento personalizada que se vincula al contenido. |
| [Clear](../../aspose.cells.properties/documentpropertycollection/clear)() | Elimina todas las propiedades de la colección. |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains)(string) | Devuelve verdadero si existe una propiedad con el nombre especificado en la colección. |
| [GetEnumerator](../../aspose.cells.properties/documentpropertycollection/getenumerator)() |  |
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof)(string) | Obtiene el índice de una propiedad por nombre. |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove)(string) | Elimina una propiedad con el nombre especificado de la colección. |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat)(int) | Elimina una propiedad en el índice especificado. |
| [UpdateLinkedPropertyValue](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue)() | Actualice el valor de la propiedad del documento personalizado que vincula al contenido. |
| [UpdateLinkedRange](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange)() | Actualice el valor de la propiedad del documento personalizado al rango vinculado. |

### Observaciones

Cada[`DocumentProperty`](../documentproperty) object representa una propiedad personalizada de un documento contenedor.

### Ejemplos

```csharp

[C#]

//Crear una instancia de un objeto Workbook
Workbook workbook = new Workbook("book1.xls");

//Recuperar una lista de todas las propiedades del documento personalizado del archivo de Excel
CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

[VB.NET]

'Crear una instancia de un objeto Workbook
Dim workbook As New Workbook("book1.xls")

'Recuperar una lista de todas las propiedades del documento personalizado del archivo de Excel
Dim customProperties As CustomDocumentPropertyCollection = workbook.Worksheets.CustomDocumentProperties

```

### Ver también

* class [DocumentPropertyCollection](../documentpropertycollection)
* espacio de nombres [Aspose.Cells.Properties](../../aspose.cells.properties)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
