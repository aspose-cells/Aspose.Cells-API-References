##Aspose::Cells::TxtLoadOptions::SetMaxRowCount method
'Aspose::Cells::TxtLoadOptions::SetMaxRowCount method. The maximum count of rows to be imported for one sheet in C++.'
## TxtLoadOptions::SetMaxRowCount method
The maximum count of rows to be imported for one sheet.
```cpp
void Aspose::Cells::TxtLoadOptions::SetMaxRowCount(int32_t value)
```
## Remarks
Those rows exceeding this limit will be ignored or extended to next sheet according to ExtendToNextSheet. This count includes the header rows(HeaderRowsCount). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
## See Also
* Class [Vector](../../vector/)
* Class [TxtLoadOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
