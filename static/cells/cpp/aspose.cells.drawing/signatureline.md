##Aspose::Cells::Drawing::SignatureLine class
'Aspose::Cells::Drawing::SignatureLine class. Represent the signature line in C++.'
## SignatureLine class
Represent the signature line.
```cpp
class SignatureLine
```
## Methods
| Method | Description |
| --- | --- |
| [GetAllowComments()](./getallowcomments/) | Indicates whether comments could be attached. |
| [GetEmail()](./getemail/) | Gets or sets the email of singer. |
| [GetId(UUID\& uuid)](./getid/) | Gets or sets identifier for this signature line. |
| [GetInstructions()](./getinstructions/) | Gets or sets the text shown to user at signing time. |
| [GetProviderId(UUID\& uuid)](./getproviderid/) | Gets or sets the id of signature provider. |
| [GetShowSignedDate()](./getshowsigneddate/) | Indicates whether show signed date. |
| [GetSignatureLineType()](./getsignaturelinetype/) | Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
| [GetSigner()](./getsigner/) | Gets or sets the signer. |
| [GetTitle()](./gettitle/) | Gets or sets the title of singer. |
| [IsLine()](./isline/) | Indicates whether it is a signature line. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SignatureLine\& src)](./operator_asm/) | operator= |
| [SetAllowComments(bool value)](./setallowcomments/) | Indicates whether comments could be attached. |
| [SetEmail(const U16String\& value)](./setemail/) | Gets or sets the email of singer. |
| [SetEmail(const char16_t* value)](./setemail/) | Gets or sets the email of singer. |
| [SetId(const UUID\& value)](./setid/) | Gets or sets identifier for this signature line. |
| [SetInstructions(const U16String\& value)](./setinstructions/) | Gets or sets the text shown to user at signing time. |
| [SetInstructions(const char16_t* value)](./setinstructions/) | Gets or sets the text shown to user at signing time. |
| [SetIsLine(bool value)](./setisline/) | Indicates whether it is a signature line. |
| [SetProviderId(const UUID\& value)](./setproviderid/) | Gets or sets the id of signature provider. |
| [SetShowSignedDate(bool value)](./setshowsigneddate/) | Indicates whether show signed date. |
| [SetSignatureLineType(SignatureType value)](./setsignaturelinetype/) | Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
| [SetSigner(const U16String\& value)](./setsigner/) | Gets or sets the signer. |
| [SetSigner(const char16_t* value)](./setsigner/) | Gets or sets the signer. |
| [SetTitle(const U16String\& value)](./settitle/) | Gets or sets the title of singer. |
| [SetTitle(const char16_t* value)](./settitle/) | Gets or sets the title of singer. |
| [SignatureLine()](./signatureline/) | Default constructor. |
| [SignatureLine(SignatureLine_Impl* impl)](./signatureline/) | Constructs from an implementation object. |
| [SignatureLine(const SignatureLine\& src)](./signatureline/) | Copy constructor. |
| [~SignatureLine()](./~signatureline/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
// Create signature line object
SignatureLine s;
s.SetSigner("Simon Zhao");
s.SetTitle("Development Lead");
s.SetEmail("Simon.Zhao@aspose.com");
s.SetInstructions("Sign to confirm the excel content.");
// Adds a Signature Line to the worksheet.
Picture signatureLine = worksheet.GetShapes().AddSignatureLine(0, 0, s);
//Save the excel file.
workbook.Save("result.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
