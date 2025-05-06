---
title: PivotTable.AddFieldToArea
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Adds the field to the specific area
type: docs
url: /net/aspose.cells.pivot/pivottable/addfieldtoarea/
---
## AddFieldToArea(PivotFieldType, string) {#addfieldtoarea_2}

Adds the field to the specific area.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, string fieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| fieldName | String | The name in the base fields. |

### Return Value

The field position in the specific fields.If there is no field named as it, return -1.

### Examples

```csharp
// Called: pivotTable.AddFieldToArea(PivotFieldType.Row, &amp;quot;Region&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CellsJava45386.xlsx&quot;);

            //Change the position of the newly created pivot table so that it does not overlap with the existing pivot table position
            workbook.Worksheets.Add(&quot;PIVOT3&quot;);
            Worksheet sheet = workbook.Worksheets[&quot;PIVOT3&quot;];
            sheet.PivotTables.Add(&quot;=PolicyData!tblPolicies&quot;, &quot;B3&quot;, &quot;P_PIVOT_3&quot;);
            PivotTable pivotTable = sheet.PivotTables[0];
            pivotTable.IsGridDropZones = (true);//to automatically enable drag and drop of pivot fields 
            //interpreter.addPivotCalculatedDataField(&quot;PIVOT3&quot;, &quot;P_PIVOT_3&quot;, &quot;CalculatedField1&quot;, &quot;= Construction - BusinessType&quot;, &quot;# ### ### ##0.#&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Page, &quot;Expiry&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Page, &quot;Flood&quot;);

            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Location&quot;);

            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Construction&quot;);
            pivotTable.AddCalculatedField(&quot;CalculatedField1&quot;, &quot;= Construction - BusinessType&quot;, true);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Region&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Column, &quot;State&quot;);

            workbook.Worksheets.Add(&quot;PIVOT3_copy_after_creation&quot;);

            Worksheet targetSheet = workbook.Worksheets[&quot;PIVOT3_copy_after_creation&quot;];
            targetSheet.Copy(sheet);
            targetSheet.RefreshPivotTables();
            PivotTable pt = targetSheet.PivotTables[0];
            Assert.AreEqual(3, pt.RowFields.Count);
            Assert.IsTrue(pt.DataField != null);

            workbook.Save(Constants.PivotTableDestPath + &quot;CellsJava45386.xlsx&quot;);
            //&lt;i r=&quot;1&quot; i=&quot;1&quot;&gt;
            bool c = ManualFileUtil.ManualCheckStringInZip(Constants.PivotTableDestPath + @&quot;CellsJava45386.xlsx&quot;, &quot;xl/pivotTables/pivotTable1.xml&quot;, new string[] { &quot;&lt;i r=\&quot;1\&quot; i=\&quot;1\&quot;&gt;&quot; }, true);
            Assert.IsTrue(c);

        }
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldToArea(PivotFieldType, int) {#addfieldtoarea_1}

Adds the field to the specific area.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| baseFieldIndex | Int32 | The field index in the base fields. |

### Return Value

The field position in the specific fields.

### Examples

```csharp
// Called: int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 3);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSJAVA45772.xlsx&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            PivotTableCollection pivotTables = sheet.PivotTables;

            int index = pivotTables.Add(&quot;=Sheet1!A1:D6&quot;, &quot;I1&quot;, &quot;PivotTable1&quot;);

            PivotTable pivotTable = pivotTables[index];

            pivotTable.AddFieldToArea(PivotFieldType.Data, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Page, 2);
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 3);

            pivotTable.RowFields[rowFieldIndex].ShowInOutlineForm = (true);
            pivotTable.RowFields[rowFieldIndex].ShowCompact = (true);
            pivotTable.ColumnFields[columnFieldIndex].ShowInOutlineForm = (true);
            pivotTable.ColumnFields[columnFieldIndex].ShowCompact = (true);

            ArrayList groupByList = new ArrayList();
            groupByList.Add(PivotGroupByType.Hours);
            groupByList.Add(PivotGroupByType.Months);
            groupByList.Add(PivotGroupByType.Minutes);
            groupByList.Add(PivotGroupByType.Quarters);
            groupByList.Add(PivotGroupByType.Seconds);
            groupByList.Add(PivotGroupByType.Days);
            groupByList.Add(PivotGroupByType.Years);

            DateTime startDate = new DateTime(2008, 1, 13, 0, 32, 14);//     sdf.parse(&quot;1/13/2008 00:32:14&quot;));
            DateTime endDate = new DateTime(2014, 7, 5, 1, 0, 0);// sdf.parse(&quot;7/5/2014 01:00:00&quot;));
            pivotTable.SetManualGroupField(pivotTable.BaseFields[1], startDate, endDate, groupByList, 1);
            Assert.AreEqual(&quot;&lt;2008-01-13&quot;, pivotTable.BaseFields[6].PivotItems[0].GetStringValue());
            //groupByList = new ArrayList();
            //groupByList.Add(PivotGroupByType.RangeOfValues);
            //pivotTable.SetManualGroupField(pivotTable.BaseFields[3], 1.1, 9.54, groupByList, 0.235);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSJAVA45772.xlsx&quot;);
        }
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldToArea(PivotFieldType, PivotField) {#addfieldtoarea}

Adds the field to the specific area.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, PivotField pivotField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | the fields area type. |
| pivotField | PivotField | the field in the base fields. |

### Return Value

the field position in the specific fields.

### Examples

```csharp
// Called: pivot.AddFieldToArea(PivotFieldType.Column, pivot.DataField);
[Test]
        public void Method_PivotField_()
        {
            Console.WriteLine(&quot;Method_PivotField_()&quot;);
            string infn = path + &quot;Test_PivotChart.xlsx&quot;;
            string outfn = Constants.destPath + &quot;Test_PivotChart_out.xlsx&quot;;

            Workbook wb = new Workbook(infn);
            Worksheet wsPivot = wb.Worksheets[&quot;Pivot&quot;];
            Worksheet wsData = wb.Worksheets[&quot;Data&quot;];
            Aspose.Cells.Range dataRange = wsData.Cells.CreateRange(0, 0, 9, 6);
            dataRange.Name = &quot;DataRange&quot;;

            int pivotIndex = wsPivot.PivotTables.Add(dataRange.Name,
                                0,
                                0,
                                &quot;PivotTableAuto&quot;);
            PivotTable pivot = wsPivot.PivotTables[pivotIndex];
            for (int i = 0; i &lt; pivot.BaseFields.Count; i++)
            {
                PivotField field = (PivotField)pivot.BaseFields[i];
                field.DisplayName = field.Name;
                field.IsAutoSubtotals = false;
                field.ShowInOutlineForm = true;
                field.ShowCompact = false;

                if (pivot.RowFields.Count &lt; 1)
                {
                    pivot.AddFieldToArea(PivotFieldType.Row, field);
                    continue;
                }

                pivot.AddFieldToArea(PivotFieldType.Data, field);
            }

            pivot.AddFieldToArea(PivotFieldType.Column, pivot.DataField);
            pivot.IsAutoFormat = true;
            pivot.AutoFormatType = PivotTableAutoFormatType.Classic;
            pivot.ShowRowGrandTotals = false;
            pivot.DataField.ShowInOutlineForm = true;
            pivot.DataField.ShowCompact = false;

            int chartIx = wsPivot.Charts.Add(ChartType.Column, pivot.TableRange2.EndRow + 2, 0, pivot.TableRange2.EndRow + 20, pivot.TableRange2.EndColumn);
            Chart chart = wsPivot.Charts[chartIx];
            chart.PivotSource = wsPivot.Name + &quot;!&quot; + pivot.Name;

            wb.Save(outfn);
        }
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


