---
title: BeforeLoadFile
second_title: Aspose.Cells لمرجع .NET API
description: يحدث قبل تحميل المصنف من ملف.
type: docs
weight: 380
url: /ar/net/aspose.cells.griddesktop/griddesktop/beforeloadfile/
---
## GridDesktop.BeforeLoadFile event

يحدث قبل تحميل المصنف من ملف.

```csharp
public event WorkbookEventHandler BeforeLoadFile;
```

### أمثلة

```csharp
[C#]
private void gridDesktop1_BeforeLoadFile(object sender, Aspose.Cells.GridDesktop.Event.WorkBookEvents e)
{
	MessageBox.Show("before load file!");
}

[Visual Basic]
Private  Sub gridDesktop1_BeforeLoadFile(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.WorkBookEvents) Handles gridDesktop1.CellDataChanged
	MessageBox.Show("before load file!")
End Sub

```

### أنظر أيضا

* delegate [WorkbookEventHandler](../../workbookeventhandler)
* class [GridDesktop](../../griddesktop)
* مساحة الاسم [Aspose.Cells.GridDesktop](../../griddesktop)
* المجسم [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
