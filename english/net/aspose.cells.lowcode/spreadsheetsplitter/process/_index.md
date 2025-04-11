---
title: SpreadsheetSplitter.Process
second_title: Aspose.Cells for .NET API Reference
description: SpreadsheetSplitter method. Splits given template file into multiple parts
type: docs
url: /net/aspose.cells.lowcode/spreadsheetsplitter/process/
---
## Process(string, string) {#process_1}

Splits given template file into multiple parts.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be split |
| resultFile | String | The resultant file(name pattern) |

### Remarks

The output files will be build from the specified resultant file by appending sequence number of the sheet and split part. For example, if the specified output file is Split.xlsx, then the generated files will be Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...

### See Also

* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeSplitOptions) {#process}

Splits spreadsheet file into multiple parts.

```csharp
public static void Process(LowCodeSplitOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | LowCodeSplitOptions | Options for splitting spreadsheet |

### See Also

* class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


