##process method
## process(, template_file, result_file) {#System.String-System.String}
Converts template file to images.
```python
@staticmethod
def process(template_file, result_file):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| template_file | System.String | The template file to be converted to images. |
| result_file | System.String | The resultant file(name pattern) for generated images. |
### Remarks
The output files will be build from the specified result file
by appending sequence number of the sheet and split part.
For example, if the specified output file is Image.png, then the generated image
files will be Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...
## process(, load_options, save_options) {#aspose.cells.lowcode.LowCodeLoadOptions-aspose.cells.lowcode.LowCodeSaveOptions}
Converts template file to images
```python
@staticmethod
def process(load_options, save_options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| load_options | aspose.cells.lowcode.LowCodeLoadOptions | Options for input and loading |
| save_options | aspose.cells.lowcode.LowCodeSaveOptions | Options for output and saving |
### Remarks
When converting to image of format that supports multiple pages(such as tiff),
the specified [`LowCodeSaveOptions.output_file`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptions#output_file)
or [`LowCodeSaveOptions.output_stream`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptions#output_stream) will be used directly for the resultant image.
For other types of image, if the save options has specified Stream as output,
then all resultant images will be saved to the same Stream.
Otherwise, the output files will be build from the specified output file
of the save options by appending sequence number of the sheet and split part.
For example, if the specified output file is Image.png, then the generated image
files will be Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...
## process(, load_options, save_options, provider) {#aspose.cells.lowcode.LowCodeLoadOptions-aspose.cells.lowcode.LowCodeSaveOptions-Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider}
Converts template file to images
```python
@staticmethod
def process(load_options, save_options, provider):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| load_options | aspose.cells.lowcode.LowCodeLoadOptions | Options for input and loading |
| save_options | aspose.cells.lowcode.LowCodeSaveOptions | Options for saving.
| provider | Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider | Provider of save options for saving the generated images |
### See Also
* module [`aspose.cells.lowcode`](../../)
* class [`ImageConverter`](/cells/python-net/aspose.cells.lowcode/imageconverter)
