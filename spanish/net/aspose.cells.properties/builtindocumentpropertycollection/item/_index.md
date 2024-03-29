---
title: Item
second_title: Referencia de API de Aspose.Cells para .NET
description: Devuelve unDocumentPropertyaspose.cells.properties/documentproperty objeto por el nombre de la propiedad.
type: docs
weight: 110
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

Devuelve un[`DocumentProperty`](../../documentproperty) objeto por el nombre de la propiedad.

```csharp
public override DocumentProperty this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre que no distingue entre mayúsculas y minúsculas de la propiedad que se va a recuperar. |

### Observaciones

Los nombres de cadena de las propiedades corresponden a los nombres de las propiedades typed disponibles en[`BuiltInDocumentPropertyCollection`](../../builtindocumentpropertycollection).

Si solicita una propiedad que no está presente en el documento, pero el nombre de la propiedad se reconoce como un nombre incorporado válido, un nuevo[`DocumentProperty`](../../documentproperty) Se crea , se agrega a la colección y se devuelve. A la propiedad recién creada se le asigna un valor predeterminado (cadena vacía, cero, falso o DateTime.MinValue según el tipo de la propiedad integrada).

Si solicita una propiedad que no está presente en el documento y el nombre no se reconoce como un nombre incorporado, se devuelve un valor nulo.

### Ver también

* class [DocumentProperty](../../documentproperty)
* class [BuiltInDocumentPropertyCollection](../../builtindocumentpropertycollection)
* espacio de nombres [Aspose.Cells.Properties](../../builtindocumentpropertycollection)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
