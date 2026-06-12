---
title: Aspose::Cells::Worksheet::Protect method
linktitle: Protect
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Worksheet::Protect method. Protects worksheet in C++.'
type: docs
weight: 7900
url: /sv/cpp/aspose.cells/worksheet/protect/
---
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
//Instansierar ett Workbook‑objekt
Workbook excel(u"template.xlsx");
//Accessing the first worksheet in the Excel file
Worksheet worksheet = excel.GetWorksheets().Get(0);
//Skyddar kalkylbladet med ett lösenord
U16String val_1 = u"newPwd";
U16String val_2 = u"oldPwd";
worksheet.Protect(ProtectionType::All, val_1, val_2);
//Sparar den modifierade Excel-filen i standardformat (det vill säga Excel 20003)
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
//Instansierar ett Workbook‑objekt
Workbook excel(u"template.xlsx");
//Accessing the first worksheet in the Excel file
Worksheet worksheet = excel.GetWorksheets().Get(0);
//Skyddar kalkylbladet med ett lösenord
worksheet.Protect(ProtectionType::All, u"aspose", nullptr);
//Sparar den modifierade Excel-filen i standardformat (det vill säga Excel 20003)
excel.Save(u"output.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Enum [ProtectionType](../../protectiontype/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
