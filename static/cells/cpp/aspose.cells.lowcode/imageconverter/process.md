##Aspose::Cells::LowCode::ImageConverter::Process method
'Aspose::Cells::LowCode::ImageConverter::Process method. Converts template file to images in C++.'
## ImageConverter::Process(const U16String\&, const U16String\&) method
Converts template file to images.
```cpp
static void Aspose::Cells::LowCode::ImageConverter::Process(const U16String &templateFile, const U16String &resultFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | const U16String\& | The template file to be converted to images. |
| resultFile | const U16String\& | The resultant file(name pattern) for generated images. |
## Remarks
The output files will be build from the specified result file by appending sequence number of the sheet and split part. For example, if the specified output file is Image.png, then the generated image files will be Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [ImageConverter](../)
* Namespace [Aspose::Cells::LowCode](../../)
* Library [Aspose.Cells for C++](../../../)
## ImageConverter::Process(const char16_t*, const char16_t*) method
Converts template file to images.
```cpp
static void Aspose::Cells::LowCode::ImageConverter::Process(const char16_t *templateFile, const char16_t *resultFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | const char16_t* | The template file to be converted to images. |
| resultFile | const char16_t* | The resultant file(name pattern) for generated images. |
## Remarks
The output files will be build from the specified result file by appending sequence number of the sheet and split part. For example, if the specified output file is Image.png, then the generated image files will be Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageConverter](../)
* Namespace [Aspose::Cells::LowCode](../../)
* Library [Aspose.Cells for C++](../../../)
## ImageConverter::Process(const LowCodeLoadOptions\&, const LowCodeSaveOptions\&) method
Converts template file to images.
```cpp
static void Aspose::Cells::LowCode::ImageConverter::Process(const LowCodeLoadOptions &loadOptions, const LowCodeSaveOptions &saveOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | const LowCodeLoadOptions\& | Options for input and loading |
| saveOptions | const LowCodeSaveOptions\& | Options for output and saving |
## Remarks
When converting to image of format that supports multiple pages(such as tiff), the specified LowCodeSaveOptions.OutputFile or LowCodeSaveOptions.OutputStream will be used directly for the resultant image.
For other types of image, if the save options has specified Stream as output, then all resultant images will be saved to the same Stream. Otherwise, the output files will be build from the specified output file of the save options by appending sequence number of the sheet and split part. For example, if the specified output file is Image.png, then the generated image files will be Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* Class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* Class [ImageConverter](../)
* Namespace [Aspose::Cells::LowCode](../../)
* Library [Aspose.Cells for C++](../../../)
## ImageConverter::Process(const LowCodeLoadOptions\&, const LowCodeSaveOptions\&, const AbstractLowCodeSaveOptionsProvider\&) method
Converts template file to images.
```cpp
static void Aspose::Cells::LowCode::ImageConverter::Process(const LowCodeLoadOptions &loadOptions, const LowCodeSaveOptions &saveOptions, const AbstractLowCodeSaveOptionsProvider &provider)
```
| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | const LowCodeLoadOptions\& | Options for input and loading |
| saveOptions | const LowCodeSaveOptions\& | Options for saving. Its output(LowCodeSaveOptions.OutputFile or LowCodeSaveOptions.OutputStream) takes no effect because all outputs will be specified by the "provider" parameter |
| provider | const AbstractLowCodeSaveOptionsProvider\& | Provider of save options for saving the generated images |
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* Class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* Class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* Class [ImageConverter](../)
* Namespace [Aspose::Cells::LowCode](../../)
* Library [Aspose.Cells for C++](../../../)
