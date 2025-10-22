##Aspose::Cells::Charts::Series::SetName method
'Aspose::Cells::Charts::Series::SetName method. Gets or sets the name of the data series in C++.'
## Series::SetName(const U16String\&) method
Gets or sets the name of the data series.
```cpp
void Aspose::Cells::Charts::Series::SetName(const U16String &value)
```
## Examples
```cpp
//Reference name to a cell
U16String val = u"=A1";
chart.GetNSeries().Get(0).SetName(val);
//Set a string to name
val = u"First Series";
chart.GetNSeries().Get(0).SetName(val);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Series](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Series::SetName(const char16_t*) method
Gets or sets the name of the data series.
```cpp
void Aspose::Cells::Charts::Series::SetName(const char16_t *value)
```
## Examples
```cpp
//Reference name to a cell
chart.GetNSeries().Get(0).SetName(u"=A1");
//Set a string to name
chart.GetNSeries().Get(0).SetName(u"First Series");
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Series](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
