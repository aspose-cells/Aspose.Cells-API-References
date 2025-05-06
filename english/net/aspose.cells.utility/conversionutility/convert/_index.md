---
title: ConversionUtility.Convert
second_title: Aspose.Cells for .NET API Reference
description: ConversionUtility method. Converts Excel files to other formats
type: docs
url: /net/aspose.cells.utility/conversionutility/convert/
---
## Convert(string, string) {#convert_1}

Converts Excel files to other formats.

```csharp
public static void Convert(string source, string saveAs)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | String | The source file name. |
| saveAs | String | The file name of expected file. |

### Examples

```csharp
// Called: ConversionUtility.Convert(Constants.sourcePath + &amp;quot;CellsNet55498.xlsx&amp;quot;, Constants.destPath + &amp;quot;CellsNet55498.pdf&amp;quot;);
[Test]
        public void Method_String_()
        {
            ConversionUtility.Convert(Constants.sourcePath + &quot;CellsNet55498.xlsx&quot;, Constants.destPath + &quot;CellsNet55498.pdf&quot;);
        }
```

### See Also

* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## Convert(string, LoadOptions, string, SaveOptions) {#convert}

Converts Excel files to other formats.

```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs, 
    SaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | String | The source file name. |
| loadOptions | LoadOptions | The options of loading the source file. |
| saveAs | String | The file name of expected file. |
| saveOptions | SaveOptions | The options of saving the file. |

### See Also

* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


