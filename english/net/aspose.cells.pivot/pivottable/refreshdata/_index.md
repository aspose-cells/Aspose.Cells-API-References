---
title: PivotTable.RefreshData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Refreshes pivottables data and setting from its data source
type: docs
url: /net/aspose.cells.pivot/pivottable/refreshdata/
---
## RefreshData() {#refreshdata}

Refreshes pivottable's data and setting from it's data source.

```csharp
public PivotRefreshState RefreshData()
```

### Remarks

We will gather data from data source to a pivot cache ,then calculate the data in the cache to the cells. This method is only used to gather all data to a pivot cache.

### Examples

```csharp
// Called: pivotTable.RefreshData();//exception
[Test]
        public void Method_RefreshData()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET46279_";

            Workbook excelFile = new Workbook(filePath + "Bank Reconciliation.xlsb");

            foreach (Worksheet sheet in excelFile.Worksheets)
            {
                foreach (PivotTable pivotTable in sheet.PivotTables)
                {
                    pivotTable.RefreshData();//exception 
                    pivotTable.CalculateData();
                }

                foreach (Chart chart in sheet.Charts)
                {
                    chart.RefreshPivotData();
                    chart.Calculate();
                }
            }
        }
```

### See Also

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RefreshData(PivotTableRefreshOption) {#refreshdata_1}

Refreshes pivottable's data and setting from it's data source with options.

```csharp
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The options for refreshing data source of pivot table. |

### Examples

```csharp
// Called: pivotTable.RefreshData(option);
private void Method_PivotTableRefreshOption_(bool shown)
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + "CellsJava45864.xlsx");

            //  Worksheet worksheet = wb.Worksheets["PNL-Islamic"];
            Worksheet worksheet = wb.Worksheets["PNL_AFS"];
            wb.Worksheets.ActiveSheetIndex = worksheet.Index;
            if (worksheet != null)
            {
                PivotTableCollection pivotTables = worksheet.PivotTables;
                PivotTable pivotTable = pivotTables[0];
                PivotFieldCollection baseFieldCollection = pivotTable.BaseFields;
                for (int i = 0; i < baseFieldCollection.Count; i++)
                {
                    PivotField pivotField = baseFieldCollection[i];
                    //System.out.println("PivotField: " + pivotField.getName());
                    if (pivotField.Name == "Period")
                    {
                        PivotItemCollection pivotItems = pivotField.PivotItems;
                        for (int j = 0; j < pivotItems.Count; j++)
                        {
                            PivotItem pivotItem = pivotItems[j];
                            if (pivotItem != null)
                            {
                                pivotItem.Position = (0);
                            }
                        }
                        pivotField.ShowAllItems = shown;
                        pivotField.IsMultipleItemSelectionAllowed = true;
                        for (int j = 0; j < pivotItems.Count; j++)
                        {
                            PivotItem pivotItem = pivotItems[j];
                            if (pivotItem != null)
                            {
                                String pivotItemName = "";
                                if (pivotItem.Name == null)
                                {
                                    pivotItemName = "blank";
                                }
                                else
                                {
                                    pivotItemName = pivotItem.Name;
                                }
                                if ("NA" != (pivotItemName))
                                {
                                    pivotItem.IsHidden = false;
                                    //System.out.println("Selected: " + pivotItemName);
                                }
                                else
                                {
                                    pivotItem.IsHidden = true;
                                }
                            }
                        }
                    }
                }
                PivotTableRefreshOption option = new PivotTableRefreshOption();
                option.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
                pivotTable.RefreshData(option);
                pivotTable.CalculateData();
            }
            wb.Save(Constants.PivotTableDestPath + "CellsJava45864.xlsx");
            Assert.AreEqual("NA", worksheet.Cells["B3"].StringValue);

        }
```

### See Also

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


