---
title: Worksheet.Protect
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Protects worksheet
type: docs
url: /net/aspose.cells/worksheet/protect/
---
## Protect(ProtectionType) {#protect}

Protects worksheet.

```csharp
public void Protect(ProtectionType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ProtectionType | Protection type. |

### Remarks

This method protects worksheet without password. It can protect worksheet in all versions of Excel file.

### Examples

```csharp
// Called: sheet.Protect(ProtectionType.Objects);
[Test]
        public void Method_ProtectionType_()
        {
            using (var workbook = new Workbook(Constants.sourcePath + "CELLSNET-45977.xls"))
            {
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    sheet.Protect(ProtectionType.Objects);
                }

                workbook.Save(Constants.destPath + "CELLSNET-45977.xls");
            }
        }
```

### See Also

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Protect(ProtectionType, string, string) {#protect_1}

Protects worksheet.

```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ProtectionType | Protection type. |
| password | String | Password. |
| oldPassword | String | If the worksheet is already protected by a password, please supply the old password. Otherwise, you can set a null value or blank string to this parameter. |

### Remarks

This method can protect worksheet in all versions of Excel file.

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook excel = new Workbook("template.xlsx");
//Accessing the first worksheet in the Excel file
Worksheet worksheet = excel.Worksheets[0];
//Protecting the worksheet with a password
worksheet.Protect(ProtectionType.All, "aspose", null);
//Saving the modified Excel file in default (that is Excel 20003) format
excel.Save("output.xls");
//Closing the file stream to free all resources

[Visual Basic]

'Creating a file stream containing the Excel file to be opened
Dim fstream As FileStream = New FileStream("book1.xls", FileMode.Open)
'Instantiating a Workbook object and Opening the Excel file through the file stream
Dim excel As Workbook = New Workbook(fstream)
'Accessing the first worksheet in the Excel file
Dim worksheet As Worksheet = excel.Worksheets(0)
'Protecting the worksheet with a password
worksheet.Protect(ProtectionType.All, "aspose", DBNull.Value.ToString())
'Saving the modified Excel file in default (that is Excel 20003) format
excel.Save("output.xls")
'Closing the file stream to free all resources
fstream.Close()

```

### See Also

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


