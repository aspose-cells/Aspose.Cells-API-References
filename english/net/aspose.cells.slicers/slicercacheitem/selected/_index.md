---
title: SlicerCacheItem.Selected
second_title: Aspose.Cells for .NET API Reference
description: SlicerCacheItem property. Specifies whether the SlicerItem is selected or not
type: docs
url: /net/aspose.cells.slicers/slicercacheitem/selected/
---
## SlicerCacheItem.Selected property

Specifies whether the SlicerItem is selected or not.

```csharp
public bool Selected { get; set; }
```

### Examples

```csharp
// Called: item.Selected = false;
[Test]
        public void Property_Selected()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET44455_&quot;;

            Workbook wb = null;
            wb = new Workbook(filePath + &quot;issue.xlsx&quot;);
            wb.Save(CreateFolder(filePath) + &quot;issue_out.pdf&quot;);

            wb = new Workbook(filePath + &quot;aaa.xlsx&quot;);
            wb.Save(CreateFolder(filePath) + &quot;aaa_out.pdf&quot;);
            wb = new Workbook(filePath + &quot;bbb.xlsx&quot;);
            wb.Settings.GlobalizationSettings.PivotSettings = new CustomGlobal44455();
            wb.Save(CreateFolder(filePath) + &quot;bbb_out.pdf&quot;);

            #region read and write for xlsb and xlsx
            wb = new Workbook(filePath + &quot;slicer.xlsx&quot;);
            wb.Save(CreateFolder(filePath) + &quot;slicer_out.xlsx&quot;);
            wb = new Workbook(filePath + &quot;slicer.xlsb&quot;);
            wb.Save(CreateFolder(filePath) + &quot;slicer_out.xlsb&quot;);
            #endregion

            #region conversion between xlsb and xlsx
            wb = new Workbook(filePath + &quot;slicer.xlsx&quot;);
            wb.Save(CreateFolder(filePath) + &quot;slicer_out1.xlsx&quot;);
            wb.Save(CreateFolder(filePath) + &quot;slicer_out1.xlsb&quot;);//ok
            wb.Save(Constants.PivotTableDestPath + @&quot;html/NET44455_out.html&quot;);
            wb = new Workbook(filePath + &quot;slicer.xlsb&quot;);
            wb.Save(CreateFolder(filePath) + &quot;slicer_out2.xlsx&quot;);//ok
            wb.Save(CreateFolder(filePath) + &quot;slicer_out2.xlsb&quot;);
            #endregion


            #region create slicer
            wb = new Workbook(filePath + &quot;a.xlsx&quot;);
            Worksheet sheet = wb.Worksheets[0];
            PivotTable pivot = sheet.PivotTables[0];
            int index = sheet.Slicers.Add(pivot, &quot;A10&quot;, pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[index];
            slicer.NumberOfColumns = 2;
            slicer.StyleType = SlicerStyleType.SlicerStyleDark1;


            wb.Save(CreateFolder(filePath) + &quot;a_createSlicer.xlsx&quot;);
            wb.Save(CreateFolder(filePath) + &quot;a_createSlicer.xlsb&quot;);
            wb.Save(CreateFolder(filePath) + &quot;a_createSlicer.pdf&quot;);

            SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
            int itemCount = items.Count;
            for (int i = 0; i &lt; itemCount; i++)
            {
                SlicerCacheItem item = items[i];
                //only select partial items 
                if (i % 2 == 0)
                {
                    item.Selected = false;
                }
            }
            slicer.Refresh();

            wb.Save(CreateFolder(filePath) + &quot;a_updateSlicer.xlsx&quot;);
            wb.Save(CreateFolder(filePath) + &quot;a_updateSlicer.xlsb&quot;);
            wb.Save(CreateFolder(filePath) + &quot;a_updateSlicer.pdf&quot;);

            sheet.Slicers.Remove(slicer);
            wb.Save(CreateFolder(filePath) + &quot;a_removeSlicer.xlsx&quot;);
            wb.Save(CreateFolder(filePath) + &quot;a_removeSlicer.xlsb&quot;);
            wb.Save(CreateFolder(filePath) + &quot;a_removeSlicer.pdf&quot;);
            #endregion

            #region chart issue
            wb = new Workbook(filePath + &quot;chart.xlsx&quot;);
            wb.Save(CreateFolder(filePath) + &quot;chart_toXls.xls&quot;);
            #endregion
        }
```

### See Also

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


