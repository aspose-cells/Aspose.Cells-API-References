---
title: Class WorkbookMetadata
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Metadata.WorkbookMetadata class. Represents the meta data
type: docs
url: /net/aspose.cells.metadata/workbookmetadata/
---
## WorkbookMetadata class

Represents the meta data.

```csharp
public class WorkbookMetadata
```

## Constructors

| Name | Description |
| --- | --- |
| [WorkbookMetadata](workbookmetadata/#constructor)(Stream, MetadataOptions) | Create the meta data object. |
| [WorkbookMetadata](workbookmetadata/#constructor_1)(string, MetadataOptions) | Create the meta data object. |

## Properties

| Name | Description |
| --- | --- |
| [BuiltInDocumentProperties](../../aspose.cells.metadata/workbookmetadata/builtindocumentproperties/) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) collection that represents all the built-in document properties of the spreadsheet. |
| [CustomDocumentProperties](../../aspose.cells.metadata/workbookmetadata/customdocumentproperties/) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) collection that represents all the custom document properties of the spreadsheet. |
| [Options](../../aspose.cells.metadata/workbookmetadata/options/) { get; } | Gets the options of the metadata. |

## Methods

| Name | Description |
| --- | --- |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save)(Stream) | Save the modified metadata to the stream. |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save_1)(string) | Save the modified metadata to the file. |

### Examples

The following example creates a WorkbookMetadata.

```csharp
[C#]
  MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
  WorkbookMetadata meta = new WorkbookMetadata("book1.xlsx", options);
  meta.CustomDocumentProperties.Add("test", "test");
  meta.Save("book2.xlsx");
```

### See Also

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


