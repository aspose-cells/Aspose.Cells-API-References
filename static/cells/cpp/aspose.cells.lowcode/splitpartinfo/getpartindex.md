##Aspose::Cells::LowCode::SplitPartInfo::GetPartIndex method
'Aspose::Cells::LowCode::SplitPartInfo::GetPartIndex method. Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single in C++.'
## SplitPartInfo::GetPartIndex method
Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single.
```cpp
int32_t Aspose::Cells::LowCode::SplitPartInfo::GetPartIndex()
```
## Remarks
If multiple sheets need to be processed and every sheet is processed(split) separately, the part index always starts from 0 for every sheet. For example, when converting workbook to images, it represents the output page index of currently processed sheet. And -1 denotes there is only one page for current sheet.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SplitPartInfo](../)
* Namespace [Aspose::Cells::LowCode](../../)
* Library [Aspose.Cells for C++](../../../)
