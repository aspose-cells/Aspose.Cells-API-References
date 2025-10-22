##Aspose::Cells::FileFormatUtil::VerifyPassword method
'Aspose::Cells::FileFormatUtil::VerifyPassword method. Detects and returns the information about a format of an excel stored in a stream in C++.'
## FileFormatUtil::VerifyPassword(const Vector \<uint8_t\>\&, const U16String\&) method
Detects and returns the information about a format of an excel stored in a stream.
```cpp
static bool Aspose::Cells::FileFormatUtil::VerifyPassword(const Vector<uint8_t> &stream, const U16String &password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | const Vector \<uint8_t\>\& |  |
| password | const U16String\& | The password for encrypted ooxml files. |
## ReturnValue
Returns whether the password is corrected.
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FileFormatUtil](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FileFormatUtil::VerifyPassword(const Vector \<uint8_t\>\&, const char16_t*) method
Detects and returns the information about a format of an excel stored in a stream.
```cpp
static bool Aspose::Cells::FileFormatUtil::VerifyPassword(const Vector<uint8_t> &stream, const char16_t *password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | const Vector \<uint8_t\>\& |  |
| password | const char16_t* | The password for encrypted ooxml files. |
## ReturnValue
Returns whether the password is corrected.
## See Also
* Class [Vector](../../vector/)
* Class [FileFormatUtil](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
