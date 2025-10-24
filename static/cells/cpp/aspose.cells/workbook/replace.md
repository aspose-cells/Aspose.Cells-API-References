##Aspose::Cells::Workbook::Replace method
'Aspose::Cells::Workbook::Replace method. Replaces a cell''s value with a new string in C++.'
## Workbook::Replace(const U16String\&, const U16String\&) method
Replaces a cell's value with a new string.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const U16String &placeHolder, const U16String &newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const U16String\& | [Cell](../../cell/) placeholder |
| newValue | const U16String\& | String value to replace |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
U16String val_1 = u"AnOldValue";
U16String val_2 = u"NewValue";
workbook.Replace(val_1, val_2);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const char16_t*, const char16_t*) method
Replaces a cell's value with a new string.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const char16_t *placeHolder, const char16_t *newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const char16_t* | [Cell](../../cell/) placeholder |
| newValue | const char16_t* | String value to replace |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
workbook.Replace(u"AnOldValue", u"NewValue");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const U16String\&, int32_t) method
Replaces a cell's value with a new integer.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const U16String &placeHolder, int32_t newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const U16String\& | [Cell](../../cell/) placeholder |
| newValue | int32_t | Integer value to replace |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
int newVal = 100;
U16String val = u"AnOldValue";
workbook.Replace(val, newVal);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const char16_t*, int32_t) method
Replaces a cell's value with a new integer.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const char16_t *placeHolder, int32_t newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const char16_t* | [Cell](../../cell/) placeholder |
| newValue | int32_t | Integer value to replace |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
int newVal = 100;
workbook.Replace(u"AnOldValue", newVal);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const U16String\&, double) method
Replaces a cell's value with a new double.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const U16String &placeHolder, double newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const U16String\& | [Cell](../../cell/) placeholder |
| newValue | double | Double value to replace |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
U16String val = u"AnOldValue";
double newVal = 100.0;
workbook.Replace(val, newVal);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const char16_t*, double) method
Replaces a cell's value with a new double.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const char16_t *placeHolder, double newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const char16_t* | [Cell](../../cell/) placeholder |
| newValue | double | Double value to replace |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
double newVal = 100.0;
workbook.Replace(u"AnOldValue", newVal);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const U16String\&, const Vector \<U16String\>\&, bool) method
Replaces a cell's value with a new string array.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const U16String &placeHolder, const Vector<U16String> &newValues, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const U16String\& | [Cell](../../cell/) placeholder |
| newValues | const Vector \<U16String\>\& | String array to replace |
| isVertical | bool | True - Vertical, False - Horizontal |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
U16String val = u"AnOldValue";
Vector<U16String> newVals{ u"Tom", u"Alice", u"Jerry" };
workbook.Replace(val, newVals, true);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const char16_t*, const Vector \<U16String\>\&, bool) method
Replaces a cell's value with a new string array.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const char16_t *placeHolder, const Vector<U16String> &newValues, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const char16_t* | [Cell](../../cell/) placeholder |
| newValues | const Vector \<U16String\>\& | String array to replace |
| isVertical | bool | True - Vertical, False - Horizontal |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
Vector<U16String> newVals{ u"Tom", u"Alice", u"Jerry" };
workbook.Replace(u"AnOldValue", newVals, true);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const U16String\&, const Vector \<int32_t\>\&, bool) method
Replaces cells' values with an integer array.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const U16String &placeHolder, const Vector<int32_t> &newValues, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const U16String\& | [Cell](../../cell/) placeholder |
| newValues | const Vector \<int32_t\>\& | Integer array to replace |
| isVertical | bool | True - Vertical, False - Horizontal |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
U16String val = u"AnOldValue";
Vector<int> newVals{ 1, 2, 3 };
workbook.Replace(val, newVals, true);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const char16_t*, const Vector \<int32_t\>\&, bool) method
Replaces cells' values with an integer array.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const char16_t *placeHolder, const Vector<int32_t> &newValues, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const char16_t* | [Cell](../../cell/) placeholder |
| newValues | const Vector \<int32_t\>\& | Integer array to replace |
| isVertical | bool | True - Vertical, False - Horizontal |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
Vector<int> newVals{ 1, 2, 3 };
workbook.Replace(u"AnOldValue", newVals, true);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const U16String\&, const Vector \<double\>\&, bool) method
Replaces cells' values with a double array.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const U16String &placeHolder, const Vector<double> &newValues, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const U16String\& | [Cell](../../cell/) placeholder |
| newValues | const Vector \<double\>\& | Double array to replace |
| isVertical | bool | True - Vertical, False - Horizontal |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
U16String val = u"AnOldValue";
Vector<double> newVals{ 1.23, 2.56, 3.14159 };
workbook.Replace(val, newVals, true);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const char16_t*, const Vector \<double\>\&, bool) method
Replaces cells' values with a double array.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const char16_t *placeHolder, const Vector<double> &newValues, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const char16_t* | [Cell](../../cell/) placeholder |
| newValues | const Vector \<double\>\& | Double array to replace |
| isVertical | bool | True - Vertical, False - Horizontal |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
//......
Vector<double> newVals{ 1.23, 2.56, 3.14159 };
workbook.Replace(u"AnOldValue", newVals, true);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(bool, const Aspose::Cells::Object\&) method
Replaces cells' values with new data.
```cpp
int32_t Aspose::Cells::Workbook::Replace(bool boolValue, const Aspose::Cells::Object &newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | bool | The boolean value to be replaced. |
| newValue | const Aspose::Cells::Object\& | New value. Can be string, integer, double or DateTime value. |
## See Also
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(int32_t, const Aspose::Cells::Object\&) method
Replaces cells' values with new data.
```cpp
int32_t Aspose::Cells::Workbook::Replace(int32_t intValue, const Aspose::Cells::Object &newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| intValue | int32_t | The integer value to be replaced. |
| newValue | const Aspose::Cells::Object\& | New value. Can be string, integer, double or DateTime value. |
## See Also
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const U16String\&, const U16String\&, const ReplaceOptions\&) method
Replaces a cell's value with a new string.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const U16String &placeHolder, const U16String &newValue, const ReplaceOptions &options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const U16String\& | [Cell](../../cell/) placeholder |
| newValue | const U16String\& | String value to replace |
| options | const ReplaceOptions\& | The replace options |
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [ReplaceOptions](../../replaceoptions/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::Replace(const char16_t*, const char16_t*, const ReplaceOptions\&) method
Replaces a cell's value with a new string.
```cpp
int32_t Aspose::Cells::Workbook::Replace(const char16_t *placeHolder, const char16_t *newValue, const ReplaceOptions &options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | const char16_t* | [Cell](../../cell/) placeholder |
| newValue | const char16_t* | String value to replace |
| options | const ReplaceOptions\& | The replace options |
## See Also
* Class [Vector](../../vector/)
* Class [ReplaceOptions](../../replaceoptions/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
