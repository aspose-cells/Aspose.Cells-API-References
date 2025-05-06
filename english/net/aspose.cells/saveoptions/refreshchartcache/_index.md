---
title: SaveOptions.RefreshChartCache
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Indicates whether refreshing chart cache data
type: docs
url: /net/aspose.cells/saveoptions/refreshchartcache/
---
## SaveOptions.RefreshChartCache property

Indicates whether refreshing chart cache data

```csharp
public bool RefreshChartCache { get; set; }
```

### Examples

```csharp
// Called: var saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx) { RefreshChartCache = true };
[Test]
        public void Property_RefreshChartCache()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-49742.xlsx&quot;);
            var saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx) { RefreshChartCache = true };
            workbook.Save(Constants.destPath + &quot;CELLSNET-49742_Resave.xlsx&quot;, saveOptions);
            string text = string.Empty;
            using (FileStream fs = File.OpenRead(workbook.FileName))
            {
                Aspose.Cells.Zip.ZipFile zipFile = Aspose.Cells.Zip.ZipFile.Read(fs);
                Aspose.Cells.Zip.ZipEntry en = zipFile.GetEntry(&quot;xl/charts/chart1.xml&quot;);
                System.IO.Stream s = zipFile.GetInputStream(en);
                StreamReader rdr = new StreamReader(s, Encoding.UTF8);
                text = rdr.ReadToEnd();
            }
            System.Xml.Linq.XDocument xdoc = System.Xml.Linq.XDocument.Parse(text);
            System.Xml.Linq.XNamespace np = &quot;http://schemas.openxmlformats.org/drawingml/2006/chart&quot;;
            System.Xml.Linq.XNamespace c15 = &quot;http://schemas.microsoft.com/office/drawing/2012/chart&quot;;
            var xExts = xdoc.Root.Element(np + &quot;chart&quot;).Element(np + &quot;plotArea&quot;).Element(np + &quot;barChart&quot;).Element(np + &quot;ser&quot;).Element(np + &quot;extLst&quot;).Elements(np + &quot;ext&quot;).GetEnumerator();
            while (xExts.MoveNext())
            {
                if (xExts.Current.Attribute(&quot;uri&quot;).Value != &quot;{02D57815-91ED-43cb-92C2-25804820EDAC}&quot;)
                    continue;
                var xEle = xExts.Current.Element(c15 + &quot;datalabelsRange&quot;).Element(c15 + &quot;dlblRangeCache&quot;);
                var xPt = xEle.Elements(np + &quot;pt&quot;).GetEnumerator();
                xPt.MoveNext();
                Assert.AreEqual(&quot;MEUR 19&quot;, xPt.Current.Element(np + &quot;v&quot;).Value, &quot;dlblRangeCache pt value&quot;);
                xPt.MoveNext();
                Assert.AreEqual(&quot;MEUR 24&quot;, xPt.Current.Element(np + &quot;v&quot;).Value, &quot;dlblRangeCache pt value&quot;);
            }
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


