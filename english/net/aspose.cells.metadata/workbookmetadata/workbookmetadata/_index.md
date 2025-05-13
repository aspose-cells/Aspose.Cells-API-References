---
title: WorkbookMetadata.WorkbookMetadata
second_title: Aspose.Cells for .NET API Reference
description: WorkbookMetadata constructor. Create the meta data object
type: docs
url: /net/aspose.cells.metadata/workbookmetadata/workbookmetadata/
---
## WorkbookMetadata(string, MetadataOptions) {#constructor_1}

Create the meta data object.

```csharp
public WorkbookMetadata(string fileName, MetadataOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String |  |
| options | MetadataOptions |  |

### Examples

```csharp
// Called: WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + "example.xls", new MetadataOptions(MetadataType.DocumentProperties));
public void WorkbookMetadata_Constructor()
{
    WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + "example.xls", new MetadataOptions(MetadataType.DocumentProperties));
}
```

### See Also

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookMetadata(Stream, MetadataOptions) {#constructor}

Create the meta data object.

```csharp
public WorkbookMetadata(Stream stream, MetadataOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream |  |
| options | MetadataOptions |  |

### See Also

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


