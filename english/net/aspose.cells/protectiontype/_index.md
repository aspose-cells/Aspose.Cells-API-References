---
title: Enum ProtectionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ProtectionType enum. Represents workbook/worksheet protection type
type: docs
url: /net/aspose.cells/protectiontype/
---
## ProtectionType enumeration

Represents workbook/worksheet protection type.

```csharp
public enum ProtectionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| All | `0` | Represents to protect all. |
| Contents | `1` | Represents to protect contents, used in Worksheet protection. |
| Objects | `2` | Represents to protect objects, used in Worksheet protection. |
| Scenarios | `3` | Represents to protect scenarios, used in Worksheet protection. |
| Structure | `4` | Represents to protect structure, used in Workbook protection. |
| Windows | `5` | Represents to protect window, used in Workbook protection. |
| None | `6` | Represents no protection. Only for Reading property. |

### Examples

```csharp
// Called: sheet.Protect(ProtectionType.All);
public void Cells_Type_ProtectionType()
{
    MemoryStream ms = new MemoryStream();
    Random r = new Random();
    int c = 0;
    for (int i = 0; i < 100; i++)
    {
        Workbook wb = new Workbook(FileFormatType.Excel97To2003);
        Worksheet sheet = wb.Worksheets[0];
        sheet.Protect(ProtectionType.All);
        int flag = r.Next(0xFFFF);
        if ((flag & 0x1C) == 0)
        {
            c++;
        }
        SetProtection(sheet.Protection, flag);
        ms.SetLength(0);
        wb.Save(ms, SaveFormat.Excel97To2003);
        ms.Seek(0, SeekOrigin.Begin);
        wb = new Workbook(ms);
        int flag1 = GetProtectionFlag(wb.Worksheets[0].Protection);
        if (flag != flag1)
        {
            Assert.Fail("Protection flags expected "
                + flag.ToString("X") + " but was " + flag1.ToString("X"));
        }
    }
    Console.WriteLine("Total " + c + " cases for all Editing properties being false");
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


