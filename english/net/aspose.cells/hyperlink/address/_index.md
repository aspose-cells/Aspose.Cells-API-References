---
title: Hyperlink.Address
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Represents the address of a hyperlink
type: docs
url: /net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

Represents the address of a hyperlink.

```csharp
public string Address { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("She.et1", workbook.Worksheets[1].Hyperlinks[0].Address);
[Test]
        public void Property_Address()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET49014.xlsx");
           Assert.AreEqual(7,workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).EndRow);
            Assert.AreEqual("=She.et1!$E$3:$G$5", workbook.Worksheets.Names[0].RefersTo);
            Assert.AreEqual("=She.et1!$C$15:$E$16", workbook.Worksheets.Names[1].RefersTo);
            Assert.AreEqual("She.et1", workbook.Worksheets[1].Hyperlinks[0].Address);
            workbook.Save(Constants.destPath + "CELLSNET49014.ods");
            workbook = new Workbook(Constants.destPath + "CELLSNET49014.ods");
            Assert.AreEqual(7, workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).EndRow);
            Assert.AreEqual("=She.et1!$E$3:$G$5", workbook.Worksheets.Names[0].RefersTo);
            Assert.AreEqual("=She.et1!$C$15:$E$16", workbook.Worksheets.Names[1].RefersTo);
            Assert.AreEqual("She.et1", workbook.Worksheets[1].Hyperlinks[0].Address);
            workbook.Save(Constants.destPath + "CELLSNET49014.ods");
            using (FileStream fs = File.OpenRead(Constants.destPath + "CELLSNET49014.ods"))
            {
                ZipFile zipFile = ZipFile.Read(fs);
                ZipEntry en = zipFile.GetEntry("content.xml");
                System.IO.Stream s = zipFile.GetInputStream(en);
                StreamReader rdr = new StreamReader(s, Encoding.UTF8);
                String text = rdr.ReadToEnd();
                Assert.AreEqual(-1, text.IndexOf("\"She.et1.B3\""));
                Assert.IsTrue(text.IndexOf("xlink:href=\"#She.et1\"") != -1);//CELLSNET-49013
            }
               
        }
```

### See Also

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


