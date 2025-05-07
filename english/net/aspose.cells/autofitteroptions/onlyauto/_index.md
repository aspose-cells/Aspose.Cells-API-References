---
title: AutoFitterOptions.OnlyAuto
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Indicates whether only fit the rows which height are not customed
type: docs
url: /net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

Indicates whether only fit the rows which height are not customed.

```csharp
public bool OnlyAuto { get; set; }
```

### Examples

```csharp
// Called: options.OnlyAuto = true;
[Test]
        public void Property_OnlyAuto()
        {
            Workbook workbook = new Workbook();

            Worksheet sheet = workbook.Worksheets[0];

            Style style = sheet.Cells[0, 0].GetStyle();
            style.IsTextWrapped = true;
            style.Font.Name = "DINPro-Regular";
            style.Font.Size = 8;

            sheet.Cells.Columns[0].Width = 18;

            sheet.Cells[0, 0].SetStyle(style);

            sheet.Cells[0, 0].Value = "Furor-Bet. frei (NG f. KW 10)" + Environment.NewLine +
                "306 ÜN Lena Kern(Mo - So)" + Environment.NewLine +
                Environment.NewLine +
                "Tcherniradev, Overbeck, Kuznick, Ballhaus, Stojanowa, Burmester, Buchwald, Helbig, Schubert, Sählbrandt, Richter, Andreew, Trabichoff, Castagner ab 17:30";

            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            workbook.Worksheets[0].AutoFitRows(options);
            workbook.Save(Constants.destPath + "CELLSNET47740.xlsx");
            Assert.AreEqual(195, sheet.Cells.GetRowHeightPixel(0));
        }
```

### See Also

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


