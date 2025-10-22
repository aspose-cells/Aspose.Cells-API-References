##SplitPartInfo.PartIndex
SplitPartInfo property. Index of current part in sequence0 based. 1 means there are no multiple parts so the result is single
## SplitPartInfo.PartIndex property
Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single.
```csharp
public int PartIndex { get; }
```
### Remarks
If multiple sheets need to be processed and every sheet is processed(split) separately, the part index always starts from 0 for every sheet. For example, when converting workbook to images, it represents the output page index of currently processed sheet. And -1 denotes there is only one page for current sheet.
### See Also
* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
