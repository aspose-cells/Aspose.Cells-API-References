##Aspose::Cells::Workbook::UpdateLinkedDataSource method
'Aspose::Cells::Workbook::UpdateLinkedDataSource method. If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data from give sources in C++.'
## Workbook::UpdateLinkedDataSource method
If this workbook contains external links to other data source, [Aspose.Cells](../../) will attempt to retrieve the latest data from give sources.
```cpp
void Aspose::Cells::Workbook::UpdateLinkedDataSource(const Vector<Workbook> &externalWorkbooks)
```
| Parameter | Type | Description |
| --- | --- | --- |
| externalWorkbooks | const Vector \<Workbook\>\& | Workbooks that will be used to update data of external links referenced by this workbook. The match of those workbooks with external links is determined by Workbook.FileName and ExternalLink.DataSource. So please make sure Workbook.FileName has been specified with the proper value for every workbook so they can be linked to corresponding external link. |
## Remarks
If corresponding external link cannot be found for one workbook, then this workbook will be ignored. So when you set a formula later with one new external link which you intend to make the ignored workbook be linked to it, the link cannot be performed until you call this this method again with those workbooks.
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
