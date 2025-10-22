##Aspose::Cells::Timelines::TimelineCollection::Get method
'Aspose::Cells::Timelines::TimelineCollection::Get method. Gets the Timeline by index in C++.'
## TimelineCollection::Get(int32_t) method
Gets the [Timeline](../../timeline/) by index.
```cpp
Timeline Aspose::Cells::Timelines::TimelineCollection::Get(int32_t index)
```
## Examples
```cpp
//Get the Timeline by index.
Timeline objByIndex = sheet.GetTimelines().Get(0);
```
## See Also
* Class [Timeline](../../timeline/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Get(const U16String\&) method
Gets the [Timeline](../../timeline/) by [Timeline](../../timeline/)'s name.
```cpp
Timeline Aspose::Cells::Timelines::TimelineCollection::Get(const U16String &name)
```
## Examples
```cpp
//Get the Timeline by Timeline's name.
U16String val = u"date";
Timeline objByName = sheet.GetTimelines().Get(val);
```
## See Also
* Class [Timeline](../../timeline/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Get(const char16_t*) method
Gets the [Timeline](../../timeline/) by [Timeline](../../timeline/)'s name.
```cpp
Timeline Aspose::Cells::Timelines::TimelineCollection::Get(const char16_t *name)
```
## Examples
```cpp
//Get the Timeline by Timeline's name.
Timeline objByName = sheet.GetTimelines().Get(u"date");
```
## See Also
* Class [Timeline](../../timeline/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
