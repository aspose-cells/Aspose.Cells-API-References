##LowCodeSaveOptionsProviderOfPlaceHolders class
## LowCodeSaveOptionsProviderOfPlaceHolders class
Implementation to provide save options which save split parts to files
and the path of resultant file are defined with placeholders.
**Inheritance:** [`LowCodeSaveOptionsProviderOfPlaceHolders`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders)
The LowCodeSaveOptionsProviderOfPlaceHolders type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self, path_template)`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/__init__/#system.string) | Instantiates an instance to provide save options according to specified templates. |
### Properties
| Property | Description |
| :- | :- |
| [sheet_index_offset](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheet_index_offset) | Offset of sheet's index between what used in file path
| [split_part_index_offset](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/split_part_index_offset) | Offset of split part's index between what used in file path
| [build_path_with_sheet_always](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/build_path_with_sheet_always) | Whether add sheet index or name to file path always.
| [build_path_with_split_part_always](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/build_path_with_split_part_always) | Whether add split part index to file path always.
| [sheet_name_prefix](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheet_name_prefix) | Prefix for the index of worksheet. |
| [sheet_index_prefix](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheet_index_prefix) | Prefix for the index of worksheet. |
| [split_part_prefix](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/split_part_prefix) | Prefix for the index of split part. |
| [save_options_template](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/save_options_template) | The template for creating instance of save options in [`LowCodeSaveOptionsProviderOfPlaceHolders.get_save_options`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/get_save_options). |
### Methods
| Method | Description |
| :- | :- |
| [`get_save_options(self, part)`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/get_save_options/#aspose.cells.lowcode.splitpartinfo) | Gets the save options from which to get the output settings for currently split part. |
| [`finish(self, part)`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/finish/#aspose.cells.lowcode.lowcodesaveoptions) |  |
### See Also
* module [`aspose.cells.lowcode`](..)
* class [`LowCodeSaveOptionsProviderOfPlaceHolders`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders)
