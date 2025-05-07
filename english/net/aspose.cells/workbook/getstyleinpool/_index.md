---
title: Workbook.GetStyleInPool
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells
type: docs
url: /net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells.

```csharp
public Style GetStyleInPool(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index. |

### Return Value

The style in the pool corresponds to given index, may be null.

### Remarks

If the returned style is changed, the style of all cells(which refers to this style) will be changed.

### Examples

```csharp
// Called: Style style = reloadWb.GetStyleInPool(i);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + "CELLSNET-49498.html");

            wb.Worksheets[0].AutoFitColumns();

            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);

                ms.Position = 0;

                Workbook reloadWb = new Workbook(ms);
                int count = reloadWb.CountOfStylesInPool;
                for (int i = 0; i < count; i++)
                {
                    Style style = reloadWb.GetStyleInPool(i);

                    string customNumberFormat = style.Custom;
                    if (!string.IsNullOrEmpty(customNumberFormat))
                    {
                        string lowerCaseCustomNumberFormat = customNumberFormat.ToLower();
                        Assert.IsTrue(lowerCaseCustomNumberFormat.IndexOf("standard") == -1);
                        Assert.IsTrue(lowerCaseCustomNumberFormat.IndexOf("short date") == -1);
                        Assert.IsTrue(lowerCaseCustomNumberFormat.IndexOf("&#39") == -1);
                    }
                }
            }
        }
```

### See Also

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


