---
title: GlobalizationSettings.GetDefaultSheetName
second_title: Aspose.Cells for .NET API Reference
description: GlobalizationSettings method. Gets the default sheet name for adding worksheet automatically. Default is Sheet
type: docs
url: /net/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings.GetDefaultSheetName method

Gets the default sheet name for adding worksheet automatically. Default is "Sheet".

```csharp
public virtual string GetDefaultSheetName()
```

### Return Value

the default sheet name for adding worksheet automatically

### Remarks

The automatically added(such as by [`Add`](../../worksheetcollection/add/)) sheet's name will be the specified name plus sequence number. For example, for Germany user maybe wants the sheet name to be "Tabellenblatt2" instead of "Sheet2". Then user may implement this method to return "Tabellenblatt".

### See Also

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


