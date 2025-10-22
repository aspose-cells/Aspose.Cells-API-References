##Aspose::Cells::AboveAverage class
'Aspose::Cells::AboveAverage class. Describe the AboveAverage conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range in C++.'
## AboveAverage class
Describe the [AboveAverage](./) conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range.
```cpp
class AboveAverage
```
## Methods
| Method | Description |
| --- | --- |
| [AboveAverage()](./aboveaverage/) | Default constructor. |
| [AboveAverage(AboveAverage_Impl* impl)](./aboveaverage/) | Constructs from an implementation object. |
| [AboveAverage(const AboveAverage\& src)](./aboveaverage/) | Copy constructor. |
| [GetStdDev()](./getstddev/) | Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0. |
| [IsAboveAverage()](./isaboveaverage/) | Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true. |
| [IsEqualAverage()](./isequalaverage/) | Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const AboveAverage\& src)](./operator_asm/) | operator= |
| [SetIsAboveAverage(bool value)](./setisaboveaverage/) | Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true. |
| [SetIsEqualAverage(bool value)](./setisequalaverage/) | Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false. |
| [SetStdDev(int32_t value)](./setstddev/) | Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0. |
| [~AboveAverage()](./~aboveaverage/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
