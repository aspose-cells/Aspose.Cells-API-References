---
title: NumbersLoadOptions.LoadTableType
second_title: Aspose.Cells for .NET API Reference
description: NumbersLoadOptions property. Gets and sets the type of loading multiple tables in one worksheet
type: docs
url: /net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

Gets and sets the type of loading multiple tables in one worksheet.

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### Examples

```csharp
// Called: numbersLoadOptions.LoadTableType = LoadNumbersTableType.TileTables;
[Test]
        public void Property_LoadTableType()
        {
            NumbersLoadOptions numbersLoadOptions = new NumbersLoadOptions();
            numbersLoadOptions.LoadTableType = LoadNumbersTableType.TileTables;
            Workbook wb = new Workbook(Constants.sourcePath + "Numbers13/CELLSNET51709.numbers", numbersLoadOptions);
            Assert.AreEqual("CA TTC", wb.Worksheets[0].Cells["B52"].StringValue);
            Util.ReSave(wb, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + "CELLSNET51709.xlsx");
        }
```

### See Also

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


