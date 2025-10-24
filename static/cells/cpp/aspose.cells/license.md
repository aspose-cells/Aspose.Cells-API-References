##Aspose::Cells::License class
'Aspose::Cells::License class. Provides methods to license the component in C++.'
## License class
Provides methods to license the component.
```cpp
class License
```
## Methods
| Method | Description |
| --- | --- |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [License()](./license/) | Default constructor. |
| [License(License_Impl* impl)](./license/) | Constructs from an implementation object. Internal use. |
| [License(const License\& src)](./license/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const License\& src)](./operator_asm/) | operator= |
| [SetLicense(const U16String\& licenseName)](./setlicense/) | Licenses the component. |
| [SetLicense(const char16_t* licenseName)](./setlicense/) | Licenses the component. |
| [SetLicense(const Vector \<uint8_t\>\& stream)](./setlicense/) | Licenses the component. |
| [~License()](./~license/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
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
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
