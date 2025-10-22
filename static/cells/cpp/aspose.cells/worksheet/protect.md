##Aspose::Cells::Worksheet::Protect method
'Aspose::Cells::Worksheet::Protect method. Protects worksheet in C++.'
## Worksheet::Protect(ProtectionType) method
Protects worksheet.
```cpp
void Aspose::Cells::Worksheet::Protect(ProtectionType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ProtectionType | [Protection](../../protection/) type. |
## Remarks
This method protects worksheet without password. It can protect worksheet in all versions of Excel file.
## See Also
* Class [Vector](../../vector/)
* Enum [ProtectionType](../../protectiontype/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::Protect(ProtectionType, const U16String\&, const U16String\&) method
Protects worksheet.
```cpp
void Aspose::Cells::Worksheet::Protect(ProtectionType type, const U16String &password, const U16String &oldPassword)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ProtectionType | [Protection](../../protection/) type. |
| password | const U16String\& | Password. |
| oldPassword | const U16String\& | If the worksheet is already protected by a password, please supply the old password. Otherwise, you can set a null value or blank string to this parameter. |
## Remarks
This method can protect worksheet in all versions of Excel file.
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook excel(u"template.xlsx");
//Accessing the first worksheet in the Excel file
Worksheet worksheet = excel.GetWorksheets().Get(0);
//Protecting the worksheet with a password
U16String val_1 = u"newPwd";
U16String val_2 = u"oldPwd";
worksheet.Protect(ProtectionType::All, val_1, val_2);
//Saving the modified Excel file in default (that is Excel 20003) format
excel.Save(u"output.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Enum [ProtectionType](../../protectiontype/)
* Class [U16String](../../u16string/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::Protect(ProtectionType, const char16_t*, const char16_t*) method
Protects worksheet.
```cpp
void Aspose::Cells::Worksheet::Protect(ProtectionType type, const char16_t *password, const char16_t *oldPassword)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ProtectionType | [Protection](../../protection/) type. |
| password | const char16_t* | Password. |
| oldPassword | const char16_t* | If the worksheet is already protected by a password, please supply the old password. Otherwise, you can set a null value or blank string to this parameter. |
## Remarks
This method can protect worksheet in all versions of Excel file.
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook excel(u"template.xlsx");
//Accessing the first worksheet in the Excel file
Worksheet worksheet = excel.GetWorksheets().Get(0);
//Protecting the worksheet with a password
worksheet.Protect(ProtectionType::All, u"aspose", nullptr);
//Saving the modified Excel file in default (that is Excel 20003) format
excel.Save(u"output.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Enum [ProtectionType](../../protectiontype/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
