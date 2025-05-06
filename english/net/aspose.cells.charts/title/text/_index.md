---
title: Title.Text
second_title: Aspose.Cells for .NET API Reference
description: Title property. Gets or sets the text of display unit label
type: docs
url: /net/aspose.cells.charts/title/text/
---
## Title.Text property

Gets or sets the text of display unit label.

```csharp
public override string Text { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].Charts[0].ValueAxis.Title.Text = &amp;quot;Alerts&amp;quot;;
[Test]
        public void Property_Text()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Excel[1].2007.Alerts.xlsx&quot;);
            workbook.Worksheets[0].Charts[0].ValueAxis.Title.Text = &quot;Alerts&quot;;

            workbook.Save(Constants.destPath + &quot;TestCellsNet13422.xlsx&quot;);
        }
```

### See Also

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


