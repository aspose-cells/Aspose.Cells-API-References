---
title: Aspose::Cells::Properties::DocumentProperty class
linktitle: DocumentProperty
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Properties::DocumentProperty class. Represents a custom or built-in document property in C++.'
type: docs
weight: 700
url: /es/cpp/aspose.cells.properties/documentproperty/
---
## DocumentProperty class


Represents a custom or built-in document property.

```cpp
class DocumentProperty
```

## Methods

| Method | Description |
| --- | --- |
| [DocumentProperty(DocumentProperty_Impl* impl)](./documentproperty/) | Constructs from an implementation object. |
| [DocumentProperty(const DocumentProperty\& src)](./documentproperty/) | Copy constructor. |
| [GetName()](./getname/) | Returns the name of the property. |
| [GetSource()](./getsource/) | The linked content source. |
| [GetType()](./gettype/) | Gets the data type of the property. |
| [GetValue()](./getvalue/) | Gets or sets the value of the property. |
| [IsGeneratedName()](./isgeneratedname/) | Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API. |
| [IsLinkedToContent()](./islinkedtocontent/) | Indicates whether this property is linked to content. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DocumentProperty\& src)](./operator_asm/) | operator= |
| [SetValue(const Aspose::Cells::Object\& value)](./setvalue/) | Gets or sets the value of the property. |
| [ToBool()](./tobool/) | Returns the property value as bool. |
| [ToDateTime()](./todatetime/) | Returns the property value as DateTime in local timezone. |
| [ToDouble()](./todouble/) | Returns the property value as double. |
| [ToInt()](./toint/) | Returns the property value as integer. |
| [ToString()](./tostring/) | Returns the property value as a string. |
| [~DocumentProperty()](./~documentproperty/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instanciar un objeto Workbook
Workbook workbook(u"book1.xls");

//Recuperar una lista de todas las propiedades de documento personalizadas del archivo Excel
DocumentPropertyCollection customProperties = workbook.GetWorksheets().GetCustomDocumentProperties();

//Accediendo a una propiedad de documento personalizada mediante el índice de la propiedad
DocumentProperty customProperty1 = customProperties.Get(3);

//Accediendo a una propiedad de documento personalizada mediante el nombre de la propiedad
DocumentProperty customProperty2 = customProperties.Get(u"Owner");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Properties](../)
* Library [Aspose.Cells for C++](../../)
