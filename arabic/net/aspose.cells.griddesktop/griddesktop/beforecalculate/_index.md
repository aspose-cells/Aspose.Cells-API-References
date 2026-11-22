---
title: "GridDesktop.BeforeCalculate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "حدث GridDesktop. يحدث قبل حساب الصيغة في دفتر العمل"
type: docs
url: /ar/net/aspose.cells.griddesktop/griddesktop/beforecalculate/
---
## GridDesktop.BeforeCalculate event

يحدث قبل حساب الصيغة في دفتر العمل.

```csharp
public event WorkbookEventHandler BeforeCalculate;
```

### أمثلة

```csharp
[C#]
private void gridDesktop1_BeforeCalculate(object sender, Aspose.Cells.GridDesktop.Event.WorkBookEvents e)
{
	MessageBox.Show("before calculate formula!");
}

[Visual Basic]
Private  Sub gridDesktop1_BeforeCalculate(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.WorkBookEvents) Handles gridDesktop1.CellDataChanged
	MessageBox.Show("before calculate formula!")
End Sub

```

### انظر أيضًا

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


