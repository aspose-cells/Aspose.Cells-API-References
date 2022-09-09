---
title: DocumentPropertyCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Clase base paraBuiltInDocumentPropertyCollection./builtindocumentpropertycollection yCustomDocumentPropertyCollection./customdocumentpropertycollection colecciones.
type: docs
weight: 4870
url: /es/net/aspose.cells.properties/documentpropertycollection/
---
## DocumentPropertyCollection class

Clase base para[`BuiltInDocumentPropertyCollection`](../builtindocumentpropertycollection) y[`CustomDocumentPropertyCollection`](../customdocumentpropertycollection) colecciones.

```csharp
public abstract class DocumentPropertyCollection : IEnumerable
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
| [Clear](../../aspose.cells.properties/documentpropertycollection/clear)() | Elimina todas las propiedades de la colección. |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains)(string) | Devuelve verdadero si existe una propiedad con el nombre especificado en la colección. |
| [GetEnumerator](../../aspose.cells.properties/documentpropertycollection/getenumerator)() |  |
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof)(string) | Obtiene el índice de una propiedad por nombre. |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove)(string) | Elimina una propiedad con el nombre especificado de la colección. |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat)(int) | Elimina una propiedad en el índice especificado. |

### Ejemplos

```csharp

[C#]

//Crea una instancia de un objeto Workbook llamando a su constructor vacío
Workbook workbook = new Workbook("book1.xls");
 
//Recuperar una lista de todas las propiedades del documento personalizado del archivo de Excel
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
// Acceder a una propiedad de documento personalizado usando el índice de propiedad
DocumentProperty customProperty1 = customProperties[3];
 
// Acceder a una propiedad de documento personalizado usando el nombre de la propiedad
DocumentProperty customProperty2 = customProperties["Owner"];

[VB.NET]

'Crea una instancia de un objeto Workbook llamando a su constructor vacío
Dim workbook As Workbook = New Workbook("book1.xls")
 
'Recuperar una lista de todas las propiedades del documento personalizado del archivo de Excel
Dim customProperties As DocumentPropertyCollection = workbook.Worksheets.CustomDocumentProperties
 
'Acceso a una propiedad de documento personalizado mediante el índice de propiedades
Dim customProperty1 As DocumentProperty = customProperties(3)
 
'Acceso a una propiedad de documento personalizado mediante el nombre de la propiedad
Dim customProperty2 As DocumentProperty = customProperties("Owner")

```

### Ver también

* espacio de nombres [Aspose.Cells.Properties](../../aspose.cells.properties)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->