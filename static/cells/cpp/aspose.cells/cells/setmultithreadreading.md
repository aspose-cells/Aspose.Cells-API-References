##Aspose::Cells::Cells::SetMultiThreadReading method
'Aspose::Cells::Cells::SetMultiThreadReading method. Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false in C++.'
## Cells::SetMultiThreadReading method
Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.
```cpp
void Aspose::Cells::Cells::SetMultiThreadReading(bool value)
```
## Remarks
If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by Cell.StringValue, Cell.DisplayStringValue, .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.
## See Also
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
