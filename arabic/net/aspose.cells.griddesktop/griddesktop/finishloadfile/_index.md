---
title: "GridDesktop.FinishLoadFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "حدث GridDesktop. يحدث عندما يتم تحميل دفتر العمل"
type: docs
url: /ar/net/aspose.cells.griddesktop/griddesktop/finishloadfile/
---
## GridDesktop.FinishLoadFile event

يحدث عندما يتم تحميل المصنف.

```csharp
public event WorkbookEventHandler FinishLoadFile;
```

### أمثلة

```csharp
[C#]
private void gridDesktop1_FinishLoadFile(object sender, Aspose.Cells.GridDesktop.WorkBookEvents e)
{
	MessageBox.Show("finish load file!");
}

[Visual Basic]
Private  Sub gridDesktop1_FinishLoadFile(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.WorkBookEvents) Handles gridDesktop1.FinishLoadFile
	MessageBox.Show("finish load file!")
End Sub

```

### انظر أيضًا

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


