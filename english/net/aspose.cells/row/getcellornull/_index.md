---
title: Row.GetCellOrNull
second_title: Aspose.Cells for .NET API Reference
description: Row method. Gets the cell or null in the specific index
type: docs
url: /net/aspose.cells/row/getcellornull/
---
## Row.GetCellOrNull method

Gets the cell or null in the specific index.

```csharp
public Cell GetCellOrNull(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index |

### Return Value

Returns the cell object if the cell exists. Or returns null if the cell object does not exist.

### Examples

```csharp
// Called: var tmp = tmpWb.Worksheets[0].Cells.Rows[i].GetCellOrNull(j);
private Aspose.Cells.Workbook Method_Int32_(Aspose.Cells.Workbook wb, Aspose.Cells.Range range, string cultureCode)
        {
            CultureInfo culture = CultureInfo.InvariantCulture;

            //crea un excel temporaneo in memoria e ci aggiunge un worksheet
            Aspose.Cells.Workbook tmpWb = new Aspose.Cells.Workbook();

            //recupera le celle del nuovo worksheet
            Aspose.Cells.Cells tmpCells = tmpWb.Worksheets[0].Cells;

            if (!String.IsNullOrWhiteSpace(cultureCode))
                culture = CultureInfo.CreateSpecificCulture(cultureCode);

            tmpWb.Worksheets[0].Workbook.Settings.CultureInfo = culture;
            tmpWb.Worksheets[0].IsGridlinesVisible = range.Worksheet.IsGridlinesVisible;

            //crea un range nel worksheet temporaneo e ci copia il range del file sorgente
            var tmpRange = tmpCells.CreateRange(0, 0, range.RowCount, range.ColumnCount);
            PasteOptions po = new PasteOptions()
            {
                PasteType = PasteType.Default,
                OnlyVisibleCells = true
            };
            tmpRange.Copy(range);
            tmpWb.CopyTheme(wb);

            //recupera le celle del file sorgente
            var cells = range.Worksheet.Cells;

            StyleFlag sf = new StyleFlag
            {
                All = true
            };

            for (var indexColumn = 0; indexColumn &lt; tmpRange.RowCount; indexColumn++)
            {
                tmpWb.Worksheets[0].Cells.Rows[indexColumn].Height = cells.Rows[indexColumn + range.FirstRow].Height;
            }

            for (var indexColumn = 0; indexColumn &lt; tmpRange.ColumnCount; indexColumn++)
            {
                tmpWb.Worksheets[0].Cells.Columns[indexColumn].Width = cells.Columns[indexColumn + range.FirstColumn].Width;
            }

            //cicla il range partendo della prima riga del range nel file sorgente
            for (var indexRow = tmpRange.RowCount; indexRow &gt;= 0; indexRow--)
            {
                //se la riga è nascosta o raggruppata rimuove la riga equivalente nel workesheet temporaneo
                if (cells.Rows[indexRow + range.FirstRow].IsHidden)
                {
                    tmpWb.Worksheets[0].Cells.DeleteRow(indexRow);
                }
            }

            for (var indexColumn = tmpRange.ColumnCount; indexColumn &gt;= 0; indexColumn--)
            {
                if (cells.Columns[indexColumn + range.FirstColumn].IsHidden)
                {
                    tmpWb.Worksheets[0].Cells.DeleteColumn(indexColumn);
                }
            }

            for (int i = 0; i &lt; tmpRange.RowCount; i++)
            {
                for (int j = 0; j &lt; tmpRange.RowCount; j++)
                {
                    var tmp = tmpWb.Worksheets[0].Cells.Rows[i].GetCellOrNull(j);
                    if (tmp != null)
                    {
                        if ((tmp.Type == CellValueType.IsNumeric) &amp;&amp; tmp.DisplayStringValue.EndsWith(&quot; &quot;) == true)
                        {
                            try
                            {
                                var html = tmp.HtmlString;
                                if (tmp.HtmlString.IndexOf(&quot;&amp;nbsp;&quot;) &gt;= 0)
                                {
                                    html = tmp.HtmlString.Replace(&quot;&amp;nbsp;&quot;, &quot; &quot;);
                                }

                                System.Xml.Linq.XElement x = System.Xml.Linq.XElement.Parse(html);
                                x.Value = x.Value.Replace(&quot; &quot;, &quot;[@@@]&quot;);
                                tmp.HtmlString = x.ToString();
                            }
                            catch (Exception ex)
                            {
                            }
                        }
                    }
                }
            }

            return tmpWb;
        }
```

### See Also

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


