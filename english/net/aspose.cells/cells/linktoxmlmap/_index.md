---
title: Cells.LinkToXmlMap
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Link to a xml map
type: docs
url: /net/aspose.cells/cells/linktoxmlmap/
---
## Cells.LinkToXmlMap method

Link to a xml map.

```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of xml map |
| row | Int32 | row of the destination cell |
| column | Int32 | column of the destination cell |
| path | String | path of xml element in xml map |

### Examples

```csharp
// Called: cells.LinkToXmlMap(&amp;quot;Transmittals_Map&amp;quot;, 2, 2, &amp;quot;/Transmittals/Transmittal_folder&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook(SrcPath + &quot;AddXmlMapping.xlsx&quot;);
            Worksheet sheet = wb.Worksheets[&quot;LinkToExistTable&quot;];
            Cells cells = sheet.Cells;

            cells.LinkToXmlMap(&quot;Transmittals_Map&quot;, 0, 0, &quot;/Transmittals/GUID&quot;);
            cells.LinkToXmlMap(&quot;Transmittals_Map&quot;, 4, 1, &quot;/Transmittals/Team_Member/Element&quot;);
            cells.LinkToXmlMap(&quot;Transmittals_Map&quot;, 2, 2, &quot;/Transmittals/Transmittal_folder&quot;);
            cells.LinkToXmlMap(&quot;Transmittals_Map&quot;, 1, 5, &quot;/Transmittals/Issued_Document&quot;);
            cells.LinkToXmlMap(&quot;Transmittals_Map&quot;, 3, 9, &quot;/Transmittals/Issued_Document2&quot;);

            Assert.IsTrue(cells[&quot;L1&quot;].StringValue.IndexOf(&quot;Create_User&quot;) != -1);
            Assert.AreEqual(sheet.ListObjects[&quot;Table4&quot;].EndColumn, 11);

            wb.Save(Constants.destPath + &quot;testAddXmlMappingLinkToExistTable.xlsx&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


