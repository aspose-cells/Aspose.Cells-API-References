---
title: "Clase DocumentProperty"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Properties.DocumentProperty. Representa una propiedad de documento personalizada o incorporada"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/
---
## DocumentProperty class

Representa una propiedad de documento personalizada o predefinida.

```csharp
public class DocumentProperty
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname/) { get; } | Devuelve true si esta propiedad no tiene un nombre en el almacenamiento OLE2 y se generó un nombre único solo para la API pública. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent/) { get; } | Indica si esta propiedad está vinculada al contenido |
| [Name](../../aspose.cells.properties/documentproperty/name/) { get; } | Devuelve el nombre de la propiedad. |
| [Source](../../aspose.cells.properties/documentproperty/source/) { get; } | La fuente de contenido enlazado. |
| [Type](../../aspose.cells.properties/documentproperty/type/) { get; } | Obtiene el tipo de datos de la propiedad. |
| [Value](../../aspose.cells.properties/documentproperty/value/) { get; set; } | Obtiene o establece el valor de la propiedad. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool/)() | Devuelve el valor de la propiedad como bool. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime/)() | Devuelve el valor de la propiedad como DateTime en la zona horaria local. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble/)() | Devuelve el valor de la propiedad como double. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint/)() | Devuelve el valor de la propiedad como integer. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring/)() | Devuelve el valor de la propiedad como una cadena. |

### Ejemplos

```csharp

[C#]

//Instanciar un objeto Workbook
Workbook workbook = new Workbook("book1.xls");
 
//Recuperar una lista de todas las propiedades de documento personalizadas del archivo Excel
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//Acceder a una propiedad de documento personalizada mediante el índice de la propiedad
DocumentProperty customProperty1 = customProperties[3];
 
//Acceder a una propiedad de documento personalizada mediante el nombre de la propiedad
DocumentProperty customProperty2 = customProperties["Owner"];

[VB.NET]

'Instantiate a Workbook object
Dim workbook As Workbook = New Workbook("book1.xls")
 
'Retrieve a list of all custom document properties of the Excel file
Dim customProperties As DocumentPropertyCollection = workbook.Worksheets.CustomDocumentProperties
 
'Accessng a custom document property by using the property index
Dim customProperty1 As DocumentProperty = customProperties(3)
 
'Accessng a custom document property by using the property name
Dim customProperty2 As DocumentProperty = customProperties("Owner")
```

### Ver también

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


