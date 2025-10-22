##Aspose::Cells::Cells::Find method
'Aspose::Cells::Cells::Find method. Finds the cell containing with the input object in C++.'
## Cells::Find(const Aspose::Cells::Object\&, const Cell\&) method
Finds the cell containing with the input object.
```cpp
Cell Aspose::Cells::Cells::Find(const Aspose::Cells::Object &what, const Cell &previousCell)
```
| Parameter | Type | Description |
| --- | --- | --- |
| what | const Aspose::Cells::Object\& | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | const Cell\& | Previous cell with the same object. This parameter can be set to null if searching from the start. |
## ReturnValue
[Cell](../../cell/) object.
## Remarks
Returns null (Nothing) if no cell is found.
## See Also
* Class [Cell](../../cell/)
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::Find(const Aspose::Cells::Object\&, const Cell\&, const FindOptions\&) method
Finds the cell containing with the input object.
```cpp
Cell Aspose::Cells::Cells::Find(const Aspose::Cells::Object &what, const Cell &previousCell, const FindOptions &findOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| what | const Aspose::Cells::Object\& | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | const Cell\& | Previous cell with the same object. This parameter can be set to null if searching from the start. |
| findOptions | const FindOptions\& | Find options |
## ReturnValue
[Cell](../../cell/) object.
## Remarks
Returns null (Nothing) if no cell is found.
## See Also
* Class [Cell](../../cell/)
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [FindOptions](../../findoptions/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
