##Aspose::Cells::License::SetLicense method
'Aspose::Cells::License::SetLicense method. Licenses the component in C++.'
## License::SetLicense(const U16String\&) method
Licenses the component.
```cpp
void Aspose::Cells::License::SetLicense(const U16String &licenseName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | const U16String\& | The license file path. |
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [License](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## License::SetLicense(const char16_t*) method
Licenses the component.
```cpp
void Aspose::Cells::License::SetLicense(const char16_t *licenseName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | const char16_t* | The license file path. |
## Examples
```cpp
Aspose::Cells::Startup();
//In this example, an attempt will be made to find a license file named MyLicense.lic
//in the folder that contains
License license;
license.SetLicense(u"License.lic");//your license file
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [License](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## License::SetLicense(const Vector \<uint8_t\>\&) method
Licenses the component.
```cpp
void Aspose::Cells::License::SetLicense(const Vector<uint8_t> &stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | const Vector \<uint8_t\>\& | A Vector<uint8_t> that contains the license. |
## See Also
* Class [Vector](../../vector/)
* Class [License](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
