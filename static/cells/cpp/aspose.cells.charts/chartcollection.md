##Aspose::Cells::Charts::ChartCollection class
'Aspose::Cells::Charts::ChartCollection class. Encapsulates a collection of Chart objects in C++.'
## ChartCollection class
Encapsulates a collection of [Chart](../chart/) objects.
```cpp
class ChartCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(ChartType type, int32_t upperLeftRow, int32_t upperLeftColumn, int32_t lowerRightRow, int32_t lowerRightColumn)](./add/) | Adds a chart to the collection. |
| [Add(const Vector \<uint8_t\>\& data, const U16String\& dataRange, bool isVertical, int32_t topRow, int32_t leftColumn, int32_t rightRow, int32_t bottomColumn)](./add/) | Adds a chart with preset template. |
| [Add(const Vector \<uint8_t\>\& data, const char16_t* dataRange, bool isVertical, int32_t topRow, int32_t leftColumn, int32_t rightRow, int32_t bottomColumn)](./add/) | Adds a chart with preset template. |
| [Add(ChartType type, const U16String\& dataRange, bool isVertical, int32_t topRow, int32_t leftColumn, int32_t rightRow, int32_t bottomColumn)](./add/) | Adds a chart to the collection. |
| [Add(ChartType type, const char16_t* dataRange, bool isVertical, int32_t topRow, int32_t leftColumn, int32_t rightRow, int32_t bottomColumn)](./add/) | Adds a chart to the collection. |
| [AddFloatingChart(ChartType type, int32_t left, int32_t top, int32_t width, int32_t height)](./addfloatingchart/) | Adds a chart to the collection. |
| [ChartCollection(ChartCollection_Impl* impl)](./chartcollection/) | Constructs from an implementation object. |
| [ChartCollection(const ChartCollection\& src)](./chartcollection/) | Copy constructor. |
| [Clear()](./clear/) | Clear all charts. |
| [Get(int32_t index)](./get/) | Gets the [Chart](../chart/) element at the specified index. |
| [Get(const U16String\& name)](./get/) | Gets the chart by the name. |
| [Get(const char16_t* name)](./get/) | Gets the chart by the name. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ChartCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Remove a chart at the specific index. |
| [~ChartCollection()](./~chartcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
ChartCollection charts = workbook.GetWorksheets().Get(0).GetCharts();
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
