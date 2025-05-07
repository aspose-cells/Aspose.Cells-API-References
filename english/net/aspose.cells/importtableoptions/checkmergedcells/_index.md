---
title: ImportTableOptions.CheckMergedCells
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether checking merged cells
type: docs
url: /net/aspose.cells/importtableoptions/checkmergedcells/
---
## ImportTableOptions.CheckMergedCells property

Indicates whether checking merged cells.

```csharp
public bool CheckMergedCells { get; set; }
```

### Examples

```csharp
// Called: options.CheckMergedCells = true;
[Test]
        public void Property_CheckMergedCells()
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

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


