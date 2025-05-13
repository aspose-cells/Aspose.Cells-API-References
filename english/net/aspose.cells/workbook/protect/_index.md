---
title: Workbook.Protect
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Protects a workbook
type: docs
url: /net/aspose.cells/workbook/protect/
---
## Workbook.Protect method

Protects a workbook.

```csharp
public void Protect(ProtectionType protectionType, string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| protectionType | ProtectionType | Protection type. |
| password | String | Password to protect the workbook. |

### Examples

```csharp
// Called: wbk.Protect(ProtectionType.Structure, "p");
public void Workbook_Method_Protect()
{
    Workbook wbk = new Workbook();
    wbk.Protect(ProtectionType.Structure, "p");

    wbk.Save(Constants.destPath + "example.xlsb", SaveFormat.Xlsb);
    wbk.Dispose();
}
```

### See Also

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


