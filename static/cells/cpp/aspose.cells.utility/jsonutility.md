##Aspose::Cells::Utility::JsonUtility class
'Aspose::Cells::Utility::JsonUtility class. Represents the utility class of processing json in C++.'
## JsonUtility class
Represents the utility class of processing json.
```cpp
class JsonUtility
```
## Methods
| Method | Description |
| --- | --- |
| static [ExportRangeToJson(const Range\& range, const JsonSaveOptions\& options)](./exportrangetojson/) | Exporting the range to json file. |
| static [ImportData(const U16String\& json, const Cells\& cells, int32_t row, int32_t column, const JsonLayoutOptions\& option)](./importdata/) | Import the json string. |
| static [ImportData(const char16_t* json, const Cells\& cells, int32_t row, int32_t column, const JsonLayoutOptions\& option)](./importdata/) | Import the json string. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [JsonUtility()](./jsonutility/) | Default constructor. |
| [JsonUtility(JsonUtility_Impl* impl)](./jsonutility/) | Constructs from an implementation object. |
| [JsonUtility(const JsonUtility\& src)](./jsonutility/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const JsonUtility\& src)](./operator_asm/) | operator= |
| [~JsonUtility()](./~jsonutility/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Utility](../)
* Library [Aspose.Cells for C++](../../)
