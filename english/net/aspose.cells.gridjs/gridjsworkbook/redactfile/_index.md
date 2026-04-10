---
title: GridJsWorkbook.RedactFile
second_title: Aspose.Cells for .NET API Reference
description: GridJsWorkbook method. Performs redaction on an Excel file based on an array of JSON operations
type: docs
url: /net/aspose.cells.gridjs/gridjsworkbook/redactfile/
---
## GridJsWorkbook.RedactFile method

Performs redaction on an Excel file based on an array of JSON operations.

```csharp
public void RedactFile(string excelFilePath, string uid, string[] arrayOfRedactionOpr)
```

| Parameter | Type | Description |
| --- | --- | --- |
| excelFilePath | String | The file path of the Excel file to be redacted. |
| uid | String | The unique identifier for the workbook. If null or empty, a new uid will be generated based on the file path. |
| arrayOfRedactionOpr | String[] | An array of JSON strings representing the redaction operations to be applied. |

### Exceptions

| exception | condition |
| --- | --- |
| [GridCellException](../../gridcellexception/) | Thrown when a CellsException occurs during redaction operation. |
| Exception | Thrown when a general exception occurs during redaction operation. |

### See Also

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


