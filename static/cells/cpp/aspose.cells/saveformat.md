##Aspose::Cells::SaveFormat enum
'Aspose::Cells::SaveFormat enum. Represents the format in which the workbook is saved in C++.'
## SaveFormat enum
Represents the format in which the workbook is saved.
```cpp
enum class SaveFormat
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Csv | 1 | <br>Comma-Separated [Values(CSV)](../autofilltype/) text file. |
| CSV | 1 |  **(Deprecated - Use SaveFormat.Csv instead. )** <br>Comma-Separated [Values(CSV)](../autofilltype/) text file. NOTE: This member is now obsolete. Instead, please use [Csv](../fileformattype/) property. This property will be removed 6 months later since April 2021. **Aspose** apologizes for any inconvenience you may have experienced. |
| Xlsx | 6 | <br>Represents an xlsx file. |
| Xlsm | 7 | <br>Represents an xlsm file which enable macros. |
| Xltx | 8 | <br>Represents an xltx file. |
| Xltm | 9 | <br>Represents an xltm file which enable macros. |
| Xlam | 10 | <br>Represents an xltm file which enable addin macros. |
| Tsv | 11 | <br>Tab-Separated [Values(TSV)](../autofilltype/) text file. |
| TSV | 11 |  **(Deprecated - Use FileFormatType.Tsv instead. )** <br>Tab-Separated [Values(TSV)](../autofilltype/) text file. NOTE: This member is now obsolete. Instead, please use [Tsv](../fileformattype/) property. This property will be removed 6 months later since April 2021. **Aspose** apologizes for any inconvenience you may have experienced. |
| TabDelimited | 11 | <br>Represents a tab delimited text file, same with [Tsv](../fileformattype/). |
| Html | 12 | <br>Represents a html file. |
| MHtml | 17 | <br>Represents a mhtml file. |
| Ods | 14 | <br>Open Document [Sheet(ODS)](../../aspose.cells.pivot/pivottablesourcetype/) file. |
| ODS | 14 |  **(Deprecated - Use SaveFormat.Ods instead. )** <br>Open Document [Sheet(ODS)](../../aspose.cells.pivot/pivottablesourcetype/) file. NOTE: This member is now obsolete. Instead, please use [Ods](../../aspose.cells.ods/) property. This property will be removed 6 months later since April 2021. **Aspose** apologizes for any inconvenience you may have experienced. |
| Excel97To2003 | 5 | <br>Represents an Excel97-2003 xls file. |
| SpreadsheetML | 15 | <br>Represents an Excel 2003 xml file. |
| Xlsb | 16 | <br>Represents an xlsb file. |
| Auto | 0 | <br>If saving the file to the disk,the file format accords to the extension of the file name. If saving the file to the stream, the file format is xlsx. |
| Unknown | 255 | <br>Represents unrecognized format, cannot be saved. |
| Pdf | 13 | <br>Represents a Pdf file. |
| Xps | 20 | <br>XPS (XML Paper Specification) format. |
| XPS | 20 |  **(Deprecated - Use SaveFormat.Xps instead. )** <br>XPS (XML Paper Specification) format. NOTE: This member is now obsolete. Instead, please use [Xps](../fileformattype/) property. This property will be removed 6 months later since April 2021. **Aspose** apologizes for any inconvenience you may have experienced. |
| Tiff | 21 | <br>Represents a TIFF file. |
| TIFF | 21 |  **(Deprecated - Use SaveFormat.Tiff instead. )** <br>Represents a TIFF file. NOTE: This member is now obsolete. Instead, please use [Tiff](../fileformattype/) property. This property will be removed 6 months later since April 2021. **Aspose** apologizes for any inconvenience you may have experienced. |
| Svg | 28 | <br>SVG file. |
| SVG | 28 |  **(Deprecated - Use SaveFormat.Svg instead. )** <br>SVG file. NOTE: This member is now obsolete. Instead, please use [Svg](../fileformattype/) property. This property will be removed 6 months later since April 2021. **Aspose** apologizes for any inconvenience you may have experienced. |
| Dif | 30 | <br>Data Interchange Format. |
| Ots | 31 | <br>Open Document Template [Sheet(OTS)](../../aspose.cells.pivot/pivottablesourcetype/) file. |
| Xlt | 32 | <br>Excel 97-2003 template file. |
| Xml | 51 | <br>Represents a simple xml file. |
| Numbers | 56 | <br>Represents a numbers file. |
| Markdown | 57 | <br>Represents markdown document. |
| Fods | 59 | <br>Represents OpenDocument Flat XML Spreadsheet (.fods) file format. |
| FODS | 59 |  **(Deprecated - Use SaveFormat.Fods instead. )** <br>Represents OpenDocument Flat XML Spreadsheet (.fods) file format. NOTE: This member is now obsolete. Instead, please use [Fods](../fileformattype/) property. This property will be removed 6 months later since April 2021. **Aspose** apologizes for any inconvenience you may have experienced. |
| Sxc | 60 | <br>Represents StarOffice Calc Spreadsheet (.sxc) file format. |
| SXC | 60 |  **(Deprecated - Use SaveFormat.Sxc instead. )** <br>Represents StarOffice Calc Spreadsheet (.sxc) file format. NOTE: This member is now obsolete. Instead, please use [Sxc](../fileformattype/) property. This property will be removed 6 months later since April 2021. **Aspose** apologizes for any inconvenience you may have experienced. |
| Pptx | 61 | <br>Represents .pptx file. |
| Docx | 62 | <br>Represents .docx file. |
| Emf | 258 | <br>Windows Enhanced Metafile. |
| Jpg | 261 | <br>JPEG JFIF. |
| Png | 262 | <br>Portable Network Graphics. |
| Bmp | 263 | <br>Windows Bitmap. |
| Gif | 322 | <br>Gif. |
| Json | 513 | <br>[Json](../../aspose.cells.json/). |
| SqlScript | 514 | <br>Sql. |
| XHtml | 771 |  **(Deprecated - Use HtmlVersion.XHtml instead. )** <br>Rrepesents XHtml file. please use HtmlSaveOptions.HtmlVersion property. This property will be removed 6 months later since March 2025. **Aspose** apologizes for any inconvenience you may have experienced. |
| Epub | 772 | <br>Represents Epub file. |
| Azw3 | 773 | <br>Represents Azw3 file. |
| Pcl | 1025 | <br>PCL (Printer Command Language) |
| Dbf | 515 | <br>Xbase Data file. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
