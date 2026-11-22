---
title: "GridDesktop.FinishCalculate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "حدث GridDesktop. يحدث بعد حساب الصيغة في دفتر العمل"
type: docs
url: /ar/net/aspose.cells.griddesktop/griddesktop/finishcalculate/
---
## GridDesktop.FinishCalculate event

يحدث بعد حساب الصيغة في المصنف.

```csharp
public event WorkbookEventHandler FinishCalculate;
```

### أمثلة

```csharp
[C#]
private void gridDesktop1_FinishCalculate(object sender, Aspose.Cells.GridDesktop.Event.WorkBookEvents e)
{
	MessageBox.Show("finish calculate formula!");
}

[Visual Basic]
Private  Sub gridDesktop1_FinishCalculate(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.WorkBookEvents) Handles gridDesktop1.CellDataChanged
	MessageBox.Show("finish calculate formula!")
End Sub

```

### انظر أيضًا

* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


