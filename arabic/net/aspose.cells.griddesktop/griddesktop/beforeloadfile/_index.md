---
title: "GridDesktop.BeforeLoadFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "GridDesktop حدث. يحدث قبل تحميل دفتر العمل من ملف"
type: docs
url: /ar/net/aspose.cells.griddesktop/griddesktop/beforeloadfile/
---
## GridDesktop.BeforeLoadFile event

يحدث قبل تحميل دفتر العمل من الملف.

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

### انظر أيضًا

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


