---
title: Aspose::Cells::Drawing::SignatureLine class
linktitle: SignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::SignatureLine class. Represent the signature line in C++.'
type: docs
weight: 6200
url: /cpp/aspose.cells.drawing/signatureline/
---
## SignatureLine class


Represent the signature line.

```cpp
class SignatureLine
```

## Methods

| Method | Description |
| --- | --- |
| [GetAllowComments()](./getallowcomments/) | Indicates whether comments could be attached. |
| [GetEmail()](./getemail/) | Gets and sets the email of singer. |
| [GetId(UUID\& uuid)](./getid/) | Gets or sets identifier for this signature line. |
| [GetInstructions()](./getinstructions/) | Gets and sets the text shown to user at signing time. |
| [GetProviderId(UUID\& uuid)](./getproviderid/) | Gets and sets the id of signature provider. |
| [GetShowSignedDate()](./getshowsigneddate/) | Indicates whether show signed date. |
| [GetSigner()](./getsigner/) | Gets and sets the signer. |
| [GetTitle()](./gettitle/) | Gets and sets the title of singer. |
| [IsLine()](./isline/) | Indicates whether it is a signature line. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SignatureLine\& src)](./operator_asm/) | operator= |
| [SetAllowComments(bool value)](./setallowcomments/) | Indicates whether comments could be attached. |
| [SetEmail(const U16String\& value)](./setemail/) | Gets and sets the email of singer. |
| [SetEmail(const char16_t* value)](./setemail/) | Gets and sets the email of singer. |
| [SetId(const UUID\& value)](./setid/) | Gets or sets identifier for this signature line. |
| [SetInstructions(const U16String\& value)](./setinstructions/) | Gets and sets the text shown to user at signing time. |
| [SetInstructions(const char16_t* value)](./setinstructions/) | Gets and sets the text shown to user at signing time. |
| [SetIsLine(bool value)](./setisline/) | Indicates whether it is a signature line. |
| [SetProviderId(const UUID\& value)](./setproviderid/) | Gets and sets the id of signature provider. |
| [SetShowSignedDate(bool value)](./setshowsigneddate/) | Indicates whether show signed date. |
| [SetSigner(const U16String\& value)](./setsigner/) | Gets and sets the signer. |
| [SetSigner(const char16_t* value)](./setsigner/) | Gets and sets the signer. |
| [SetTitle(const U16String\& value)](./settitle/) | Gets and sets the title of singer. |
| [SetTitle(const char16_t* value)](./settitle/) | Gets and sets the title of singer. |
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

//Adding a picture
int imgIndex = worksheet.GetPictures().Add(1, 1, u"sample.png");
Picture pic = worksheet.GetPictures().Get(imgIndex);
// Create signature line object
SignatureLine s;
s.SetSigner(u"Simon Zhao");
s.SetTitle(u"Development Lead");
s.SetEmail(u"Simon.Zhao@aspose.com");
// Assign the signature line object to Picture.SignatureLine property
pic.SetSignatureLine(s);


//Save the excel file.
workbook.Save("result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
