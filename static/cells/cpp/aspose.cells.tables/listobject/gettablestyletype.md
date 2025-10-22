##Aspose::Cells::Tables::ListObject::GetTableStyleType method
'Aspose::Cells::Tables::ListObject::GetTableStyleType method. Gets and the built-in table style in C++.'
## ListObject::GetTableStyleType method
Gets and the built-in table style.
```cpp
TableStyleType Aspose::Cells::Tables::ListObject::GetTableStyleType()
```
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook(u"Book1.xlsx");
ListObjectCollection tables = workbook.GetWorksheets().Get(0).GetListObjects();
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables.Get(0);
if (table.GetTableStyleType() != TableStyleType::TableStyleDark2)
{
table.SetTableStyleType(TableStyleType::TableStyleDark2);
}
workbook.Save(u"TableStyle.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Enum [TableStyleType](../../tablestyletype/)
* Class [ListObject](../)
* Namespace [Aspose::Cells::Tables](../../)
* Library [Aspose.Cells for C++](../../../)
