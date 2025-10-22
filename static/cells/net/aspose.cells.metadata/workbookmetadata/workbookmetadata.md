##WorkbookMetadata.WorkbookMetadata
WorkbookMetadata constructor. Create the meta data object
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
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;
namespace AsposeCellsExamples
{
public class WorkbookMetadataMethodCtorWithStringMetadataOptionsDemo
{
public static void Run()
{
string sourcePath = "example.xls";
MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);
Console.WriteLine("WorkbookMetadata created successfully with document properties metadata.");
}
}
}
```
### See Also
* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)
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
