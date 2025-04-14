---
title: ImageConverter.Process
second_title: Aspose.Cells for .NET API Reference
description: ImageConverter method. Converts template file to images
type: docs
url: /net/aspose.cells.lowcode/imageconverter/process/
---
## Process(string, string) {#process_2}

Converts template file to images.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be converted to images. |
| resultFile | String | The resultant file(name pattern) for generated images. |

### Remarks

The output files will be build from the specified result file by appending sequence number of the sheet and split part. For example, if the specified output file is Image.png, then the generated image files will be Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### See Also

* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Converts template file to images

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |

### Remarks

When converting to image of format that supports multiple pages(such as tiff), the specified [`OutputFile`](../../lowcodesaveoptions/outputfile/) or [`OutputStream`](../../lowcodesaveoptions/outputstream/) will be used directly for the resultant image.  For other types of image, if the save options has specified Stream as output, then all resultant images will be saved to the same Stream. Otherwise, the output files will be build from the specified output file of the save options by appending sequence number of the sheet and split part. For example, if the specified output file is Image.png, then the generated image files will be Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}

Converts template file to images

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeSaveOptionsProvider provider)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for saving. Its output([`OutputFile`](../../lowcodesaveoptions/outputfile/) or [`OutputStream`](../../lowcodesaveoptions/outputstream/)) takes no effect because all outputs will be specified by the "provider" parameter |
| provider | AbstractLowCodeSaveOptionsProvider | Provider of save options for saving the generated images |

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


