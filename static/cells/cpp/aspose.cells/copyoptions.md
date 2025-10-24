##Aspose::Cells::CopyOptions class
'Aspose::Cells::CopyOptions class. Represents the copy options in C++.'
## CopyOptions class
Represents the copy options.
```cpp
class CopyOptions
```
## Methods
| Method | Description |
| --- | --- |
| [CopyOptions()](./copyoptions/) | [CopyOptions](./) constructor. |
| [CopyOptions(CopyOptions_Impl* impl)](./copyoptions/) | Constructs from an implementation object. |
| [CopyOptions(const CopyOptions\& src)](./copyoptions/) | Copy constructor. |
| [GetColumnCharacterWidth()](./getcolumncharacterwidth/) | Indicates whether copying column width in unit of characters. |
| [GetCopyInvalidFormulasAsValues()](./getcopyinvalidformulasasvalues/) | If the formula is not valid for the dest destination, only copy values. |
| [GetCopyNames()](./getcopynames/) | Indicates whether copying the names. |
| [GetExtendToAdjacentRange()](./getextendtoadjacentrange/) | Indicates whether extend ranges when copying the range to adjacent range. |
| [GetKeepMacros()](./getkeepmacros/) | Indicates whether keeping macros;. |
| [GetReferToDestinationSheet()](./getrefertodestinationsheet/) | When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. |
| [GetReferToSheetWithSameName()](./getrefertosheetwithsamename/) | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const CopyOptions\& src)](./operator_asm/) | operator= |
| [SetColumnCharacterWidth(bool value)](./setcolumncharacterwidth/) | Indicates whether copying column width in unit of characters. |
| [SetCopyInvalidFormulasAsValues(bool value)](./setcopyinvalidformulasasvalues/) | If the formula is not valid for the dest destination, only copy values. |
| [SetCopyNames(bool value)](./setcopynames/) | Indicates whether copying the names. |
| [SetExtendToAdjacentRange(bool value)](./setextendtoadjacentrange/) | Indicates whether extend ranges when copying the range to adjacent range. |
| [SetKeepMacros(bool value)](./setkeepmacros/) | Indicates whether keeping macros;. |
| [SetReferToDestinationSheet(bool value)](./setrefertodestinationsheet/) | When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. |
| [SetReferToSheetWithSameName(bool value)](./setrefertosheetwithsamename/) | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. |
| [~CopyOptions()](./~copyoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
