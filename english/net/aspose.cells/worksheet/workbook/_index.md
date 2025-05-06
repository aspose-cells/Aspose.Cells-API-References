---
title: Worksheet.Workbook
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the workbook object which contains this sheet
type: docs
url: /net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

Gets the workbook object which contains this sheet.

```csharp
public Workbook Workbook { get; }
```

### Examples

```csharp
// Called: _workSheet.Cells[4, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&amp;quot;Termin Standard (TE)&amp;quot;));
[Test]
        public void Property_Workbook()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet47976.xlsx&quot;);
            Worksheet _workSheet = workbook.Worksheets[0];

            FontSetting settingText;



            _workSheet.Cells[1, 1].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Spaltentitel&quot;));
            _workSheet.Cells[1, 1].Value = &quot;Großes Haus&quot;;
            _workSheet.Cells[1, 2].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Spaltentitel&quot;));
            _workSheet.Cells[1, 2].Value = &quot;Podium&quot;;
            _workSheet.Cells[1, 3].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Spaltentitel&quot;));
            _workSheet.Cells[1, 3].Value = &quot;Uni/ BoConcept/Museum&quot;;
            _workSheet.Cells[1, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Spaltentitel&quot;));
            _workSheet.Cells[1, 4].Value = &quot;Sonstige Orte&quot;;

            _workSheet.Cells[2, 0].Value = &quot;Mo 12 Apr&quot;;
            settingText = _workSheet.Cells[2, 0].Characters(0, 2);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[2, 0].Characters(2, 3);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 12;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[2, 0].Characters(5, 4);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            string str = &quot;10:00 - 14:00 Zauberflöte Inspizienz: Goldbeck, Regieassistenz &amp; Abendspielleitung: Gentile&quot;;
            _workSheet.Cells[2, 1].Value = str;
            settingText = _workSheet.Cells[2, 1].Characters(0, 13);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[2, 1].Characters(13, 12);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[2, 1].Characters(25, 66);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[2, 2].Value = &quot;10:00 - 14:00 Scholl Regieassistenz, Abendspielleitung, Inspizienz: Halter&quot;;
            settingText = _workSheet.Cells[2, 2].Characters(0, 13);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[2, 2].Characters(13, 7);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[2, 2].Characters(20, 54);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[2, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Raum Überschrift&quot;));
            _workSheet.Cells[2, 4].Value = &quot;Messehalle 3:&quot;;
            _workSheet.Cells[3, 1].Value = &quot;18:00 - 22:00 Zauberflöte Inspizienz: Goldbeck, Regieassistenz &amp; Abendspielleitung: Gentile&quot;;
            settingText = _workSheet.Cells[3, 1].Characters(0, 13);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[3, 1].Characters(13, 12);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[3, 1].Characters(25, 66);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[3, 2].Value = &quot;18:00 - 22:00 Scholl Regieassistenz, Abendspielleitung, Inspizienz: Halter&quot;;
            settingText = _workSheet.Cells[3, 2].Characters(0, 13);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[3, 2].Characters(13, 7);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[3, 2].Characters(20, 54);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;

            _workSheet.Cells[3, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard&quot;));
            _workSheet.Cells[3, 4].Value = &quot;08:00 - 11:59 Anlieferung Lost&quot;;

            _workSheet.Cells[4, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard (TE)&quot;));
            _workSheet.Cells[4, 4].Value = &quot;12:00 - 20:00 TE Lost&quot;;

            _workSheet.Cells[5, 0].Value = &quot;Di 13 Apr&quot;;
            settingText = _workSheet.Cells[5, 0].Characters(0, 2);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[5, 0].Characters(2, 3);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 12;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[5, 0].Characters(5, 4);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[5, 1].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard&quot;));
            _workSheet.Cells[5, 1].Value = &quot;10:00 - 12:30 OA Zauberflöte&quot;;
            _workSheet.Cells[5, 2].Value = &quot;10:00 - 14:00 Scholl Regieassistenz, Abendspielleitung, Inspizienz: Halter&quot;;
            settingText = _workSheet.Cells[5, 2].Characters(0, 13);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[5, 2].Characters(13, 7);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[5, 2].Characters(20, 54);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[5, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Raum Überschrift&quot;));
            _workSheet.Cells[5, 4].Value = &quot;Oberes Foyer:&quot;;

            _workSheet.Cells[6, 1].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard&quot;));
            _workSheet.Cells[6, 1].Value = &quot;19:00 - 21:30 OA Zauberflöte&quot;;
            _workSheet.Cells[6, 2].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Vorstellung (Vst)&quot;));
            _workSheet.Cells[6, 2].Value = &quot;19:30 FÖRSTERCHRISTL&quot;;
            _workSheet.Cells[6, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard&quot;));
            _workSheet.Cells[6, 4].Value = &quot;16:00 - 17:00 Tanztheaterbande&quot;;

            _workSheet.Cells[8, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Raum Überschrift&quot;));
            _workSheet.Cells[8, 4].Value = &quot;Messehalle 3:&quot;;

            _workSheet.Cells[9, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard&quot;));
            _workSheet.Cells[9, 4].Value = &quot;08:00 - 19:00 Aufbau Lost&quot;;

            _workSheet.Cells[10, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard&quot;));
            _workSheet.Cells[10, 4].Value = &quot;19:15 - 22:00 Lost&quot;;

            _workSheet.Cells[11, 0].Value = &quot;Mi 14 Apr&quot;;
            settingText = _workSheet.Cells[11, 0].Characters(0, 2);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[11, 0].Characters(2, 3);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 12;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[11, 0].Characters(5, 4);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[11, 1].Value = &quot;10:00 - 13:00 BO Zauberflöte Inspizienz: Goldbeck, Regieassistenz &amp; Abendspielleitung: Gentile&quot;;
            settingText = _workSheet.Cells[11, 1].Characters(0, 13);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[11, 1].Characters(13, 3);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[11, 1].Characters(16, 12);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[11, 1].Characters(28, 66);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[11, 2].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Vorstellung (Vst)&quot;));
            _workSheet.Cells[11, 2].Value = &quot;19:30 COMPANY AND FRIENDS&quot;;
            _workSheet.Cells[11, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Raum Überschrift&quot;));
            _workSheet.Cells[11, 4].Value = &quot;Messehalle 3:&quot;;

            _workSheet.Cells[12, 1].Value = &quot;18:00 - 21:00 BO Zauberflöte Inspizienz: Goldbeck, Regieassistenz &amp; Abendspielleitung: Gentile&quot;;
            settingText = _workSheet.Cells[12, 1].Characters(0, 13);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[12, 1].Characters(13, 3);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[12, 1].Characters(16, 12);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[12, 1].Characters(28, 66);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[12, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard&quot;));
            _workSheet.Cells[12, 4].Value = &quot;08:00 - 19:00 Techn. Proben Lost&quot;;

            _workSheet.Cells[13, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard&quot;));
            _workSheet.Cells[13, 4].Value = &quot;19:15 - 22:00 Lost&quot;;

            _workSheet.Cells[14, 0].Value = &quot;Do 15 Apr&quot;;
            settingText = _workSheet.Cells[14, 0].Characters(0, 2);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[14, 0].Characters(2, 3);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 12;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[14, 0].Characters(5, 4);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[14, 1].Value = &quot;18:00 - 22:00 AMA Zauberflöte Inspizienz: Goldbeck, Regieassistenz &amp; Abendspielleitung: Gentile&quot;;
            settingText = _workSheet.Cells[14, 1].Characters(0, 13);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[14, 1].Characters(13, 4);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[14, 1].Characters(17, 12);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[14, 1].Characters(29, 66);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[14, 2].Value = &quot;18:00 - 22:00 Pink Guerilla Regieassistenz: Linnenlüke, Regieassistenz, Abendspielleitung, Inspizienz: Halter&quot;;
            settingText = _workSheet.Cells[14, 2].Characters(0, 13);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[14, 2].Characters(13, 14);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 10;
            settingText.Font.Color = Color.Black;
            settingText = _workSheet.Cells[14, 2].Characters(27, 82);
            settingText.Font.Name = &quot;Calibri&quot;;
            settingText.Font.DoubleSize = 8;
            settingText.Font.Color = Color.Black;
            _workSheet.Cells[14, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Raum Überschrift&quot;));
            _workSheet.Cells[14, 4].Value = &quot;Messehalle 3:&quot;;

            _workSheet.Cells[15, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard&quot;));
            _workSheet.Cells[15, 4].Value = &quot;10:00 - 14:00 Lost&quot;;

            _workSheet.Cells[16, 4].SetStyle(_workSheet.Workbook.GetNamedStyle(&quot;Termin Standard (GP)&quot;));
            _workSheet.Cells[16, 4].Value = &quot;19:00 - 22:00 GP Lost&quot;;
            workbook.Save(Constants.destPath + &quot;CellsNet47976.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet47976.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Cells[2, 1].Value , str);
        }
```

### See Also

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


