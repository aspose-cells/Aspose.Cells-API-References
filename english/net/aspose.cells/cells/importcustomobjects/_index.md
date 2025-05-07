---
title: Cells.ImportCustomObjects
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Imports custom objects
type: docs
url: /net/aspose.cells/cells/importcustomobjects/
---
## ImportCustomObjects(ICollection, string[], bool, int, int, int, bool, string, bool) {#importcustomobjects_1}

Imports custom objects.

```csharp
public int ImportCustomObjects(ICollection list, string[] propertyNames, bool isPropertyNameShown, 
    int firstRow, int firstColumn, int rowNumber, bool insertRows, string dateFormatString, 
    bool convertStringToNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| list | ICollection | The custom object |
| propertyNames | String[] | The property names.If it is null,we will import all properties of the object. |
| isPropertyNameShown | Boolean | Indicates whether the property name will be imported to the first row. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| rowNumber | Int32 | Number of rows to be imported. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |
| dateFormatString | String | Date format string for cells. |
| convertStringToNumber | Boolean | Indicates if this method will try to convert string to number. |

### Return Value

Total number of rows imported.

### Remarks

The custom objects should be the same type.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCustomObjects(ICollection, int, int, ImportTableOptions) {#importcustomobjects}

Imports custom objects.

```csharp
public int ImportCustomObjects(ICollection list, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| list | ICollection | The custom object |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| options | ImportTableOptions | The import options. |

### Return Value

Total number of rows imported.

### Remarks

The custom objects should be the same type.

### Examples

```csharp
// Called: wb.Worksheets[0].Cells.ImportCustomObjects((ICollection)customerList, 1, 0, options);
[Test]
        public void Method_ImportTableOptions_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet46711.xlsx");
            List<Customer> customerList = new List<Customer>();

            //Creating collection for test items
            for (int i = 0; i < 5; i++)
            {
                Customer customer = new Customer
                {
                    CustomerId = i,
                    Name = "Customer" + i
                };
                customerList.Add(customer);
            }
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = false;
            options.TotalRows = customerList.Count;
            options.InsertRows = true;
            options.DateFormat = "dd/mm/yyyy";
            options.ConvertNumericData = true;
            options.CheckMergedCells = true;
            //Insert data to excell
            wb.Worksheets[0].Cells.ImportCustomObjects((ICollection)customerList, 1, 0, options);
            Cell d4 = wb.Worksheets[0].Cells["D4"];
            Assert.AreEqual(d4.StringValue, "Customer2");
            Assert.IsTrue(d4.IsMerged);
            wb.Save(Constants.destPath + "CellsNet46711.xlsx", Aspose.Cells.SaveFormat.Xlsx);
        }
```

### See Also

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


