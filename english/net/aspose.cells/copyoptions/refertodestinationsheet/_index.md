---
title: CopyOptions.ReferToDestinationSheet
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. When copying the range in the same file and the chart refers to the source sheet False means the copied charts data source will not be changed. True means the copied charts data source refers to the destination sheet
type: docs
url: /net/aspose.cells/copyoptions/refertodestinationsheet/
---
## CopyOptions.ReferToDestinationSheet property

When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet.

```csharp
public bool ReferToDestinationSheet { get; set; }
```

### Remarks

The default value is false, it works as MS Excel.

### Examples

```csharp
// Called: copyOptions.ReferToDestinationSheet = true;
[Test]
        public void Property_ReferToDestinationSheet()
        {
            string outputWSName = "Output";
            int reportNum = 0;

            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ReferToDestinationSheet = true;

            Workbook tmpWorkBook = new Workbook(Constants.sourcePath + "CellsNet55472.xlsx");
            Workbook targetWB = new Workbook();
            for (int i = 0; i < 2; i++)
            {
                Worksheet sourceWS = tmpWorkBook.Worksheets[0];
                Worksheet targetWS = targetWB.Worksheets[outputWSName];
                while (targetWS != null)
                {
                    outputWSName += reportNum + 1;
                    targetWS = targetWB.Worksheets[outputWSName];
                }

                targetWS = targetWB.Worksheets.Add(outputWSName);
                targetWS.Copy(sourceWS, copyOptions);
                targetWS.PageSetup.PrintTitleRows = sourceWS.PageSetup.PrintTitleRows;
                targetWS.Cells.DeleteColumn(0);
            }
            targetWB.Save(Constants.destPath + "CellsNet55472.xlsx");
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


