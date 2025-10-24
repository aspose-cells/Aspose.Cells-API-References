##LowCodeSaveOptionsProviderOfAssembling class
## LowCodeSaveOptionsProviderOfAssembling class
Implementation to provide save options which save split parts to files
and the path of resultant file are named as(it may contains directories):
[`LowCodeSaveOptionsProviderOfAssembling.path_header`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling#path_header)+[`LowCodeSaveOptionsProviderOfAssembling.sheet_prefix`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling#sheet_prefix)+SheetIndex(or SheetName)
+[`LowCodeSaveOptionsProviderOfAssembling.split_part_prefix`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling#split_part_prefix)+SplitPartIndex+[`LowCodeSaveOptionsProviderOfAssembling.path_tail`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling#path_tail).
**Inheritance:** [`LowCodeSaveOptionsProviderOfAssembling`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling)
The LowCodeSaveOptionsProviderOfAssembling type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/__init__/#) | Constructs a new instance of LowCodeSaveOptionsProviderOfAssembling |
### Properties
| Property | Description |
| :- | :- |
| [path_header](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/path_header) | Header part(before added content of sheet and split part) of file path. |
| [path_tail](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/path_tail) | Tailing part(after sequence numbers) of file path.
| [use_sheet_name](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/use_sheet_name) | Whether builds the file path with sheet name instead of sheet index. Default value is false. |
| [sheet_prefix](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheet_prefix) | Prefix for the index of worksheet. |
| [split_part_prefix](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/split_part_prefix) | Prefix for the index of split part. |
| [sheet_index_offset](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheet_index_offset) | Offset of sheet's index between what used in file path
| [split_part_index_offset](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/split_part_index_offset) | Offset of split part's index between what used in file path
| [build_path_with_sheet_always](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/build_path_with_sheet_always) | Whether add sheet index or name to file path always.
| [build_path_with_split_part_always](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/build_path_with_split_part_always) | Whether add split part index to file path always.
| [save_options_template](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/save_options_template) | The template for creating instance of save options in [`LowCodeSaveOptionsProviderOfAssembling.get_save_options`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/get_save_options). |
### Methods
| Method | Description |
| :- | :- |
| [`get_save_options(self, part)`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/get_save_options/#aspose.cells.lowcode.splitpartinfo) | Gets the save options from which to get the output settings for currently split part. |
| [`finish(self, part)`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/finish/#aspose.cells.lowcode.lowcodesaveoptions) |  |
### See Also
* module [`aspose.cells.lowcode`](..)
* class [`LowCodeSaveOptionsProviderOfAssembling`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling)
