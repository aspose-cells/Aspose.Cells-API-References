---
title: PageSetup
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1140
url: /python-net/aspose.cells/pagesetup/
---

## PageSetup class

Encapsulates the object that represents the page setup description. <br/>            The PageSetup object contains all page setup options.

The PageSetup type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|ods_page_background|Gets the background of ODS.|
|print_area|Represents the range to be printed.|
|print_title_columns|Represents the columns that contain the cells to be repeated on the left side of each page.|
|print_title_rows|Represents the rows that contain the cells to be repeated at the top of each page.|
|black_and_white|Represents if elements of the document will be printed in black and white.|
|center_horizontally|Represent if the sheet is printed centered horizontally.|
|center_vertically|Represent if the sheet is printed centered vertically.|
|print_draft|Represents if the sheet will be printed without graphics.|
|footer_margin|Represents the distance from the bottom of the page to the footer, in unit of centimeters.|
|footer_margin_inch|Represents the distance from the bottom of the page to the footer, in unit of inches.|
|header_margin|Represents the distance from the top of the page to the header, in unit of centimeters.|
|header_margin_inch|Represents the distance from the top of the page to the header, in unit of inches.|
|printer_settings|Gets and sets the settings of the default printer.|
|left_margin|Represents the size of the left margin, in unit of centimeters.|
|left_margin_inch|Represents the size of the left margin, in unit of inches.|
|right_margin|Represents the size of the right margin, in unit of centimeters.|
|right_margin_inch|Represents the size of the right margin, in unit of inches.|
|top_margin|Represents the size of the top margin, in unit of centimeters.|
|top_margin_inch|Represents the size of the top margin, in unit of inches.|
|bottom_margin|Represents the size of the bottom margin, in unit of centimeters.|
|bottom_margin_inch|Represents the size of the bottom margin, in unit of inches.|
|first_page_number|Represents the first page number that will be used when this sheet is printed.|
|fit_to_pages_tall|Represents  the number of pages tall the worksheet will be scaled to when it's printed.<br/>            The default value is 1.|
|fit_to_pages_wide|Represents the number of pages wide the worksheet will be scaled to when it's printed.<br/>            The default value is 1.|
|is_percent_scale|If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled.|
|order|Represents the order that Microsoft Excel uses to number pages when printing a large worksheet.|
|is_automatic_paper_size|Indicates whether the paper size is automatic.|
|paper_size|Represents the size of the paper.|
|paper_width|Gets the width of the paper in unit of inches, considered page orientation.|
|paper_height|Gets the height of the paper in unit of inches , considered page orientation.|
|orientation|Represents page print orientation.|
|print_comments|Represents the way comments are printed with the sheet.|
|print_errors|Specifies the type of print error displayed.|
|print_headings|Represents if row and column headings are printed with this page.|
|print_gridlines|Represents if cell gridlines are printed on the page.|
|zoom|Represents the scaling factor in percent. It should be between 10 and 400.|
|is_auto_first_page_number|Indicates whether the first the page number is automatically assigned.|
|print_quality|Represents the print quality.|
|print_copies|Get and sets number of copies to print.|
|is_hf_diff_odd_even|True means that the header/footer of the odd pages is different with odd pages.|
|is_hf_diff_first|True means that the header/footer of the first page is different with other pages.|
|is_hf_scale_with_doc|Indicates whether header and footer are scaled with document scaling.<br/>            Only applies for Excel 2007.|
|is_hf_align_margins|Indicates whether header and footer margins are aligned with the page margins.<br/>            If this property is true, the left header and footer will be aligned with the left margin,<br/>            and the right header and footer will be aligned with the right margin.<br/>            This option is enabled by default.|
## Methods
| Name | Description |
| :- | :- |
|get_picture(is_header, section)|Gets the [Picture](/cells/python-net/aspose.cells.drawing/picture/) object of the header / footer.|
|get_picture(is_first, is_even, is_header, section)|Gets the [Picture](/cells/python-net/aspose.cells.drawing/picture/) object of the header / footer.|
|copy(source, copy_options)|Copies the setting of the page setup.|
|set_fit_to_pages(wide, tall)|Sets the number of pages the worksheet will be scaled to when it's printed.|
|custom_paper_size(width, height)|Sets the custom paper size, in unit of inches.|
|clear_header_footer()|Clears header and footer setting.|
|get_header(section)|Gets a script formatting the header of an Excel file.|
|get_commands(header_footer_script)|Gets all commands of header or footer.|
|get_footer(section)|Gets a script formatting the footer of an Excel file.|
|set_header(section, header_script)|Sets a script formatting the header of an Excel file.|
|set_footer(section, footer_script)|Sets a script formatting the footer of an Excel file.|
|set_even_header(section, header_script)|Sets a script formatting the even page header of an Excel file.<br/>            Only effect in Excel 2007 when IsHFDiffOddEven is true.|
|get_even_header(section)|Gets a script formatting the even header of an Excel file.|
|set_even_footer(section, footer_script)|Sets a script formatting the even page footer of an Excel file.<br/>            Only effect in Excel 2007 when IsHFDiffOddEven is true.|
|get_even_footer(section)|Gets a script formatting the even footer of an Excel file.|
|set_first_page_header(section, header_script)|Sets a script formatting the first page header of an Excel file.<br/>            Only effect in Excel 2007 when IsHFDiffFirst is true.|
|get_first_page_header(section)|Gets a script formatting the first page header of an Excel file.|
|set_first_page_footer(section, footer_script)|Sets a script formatting the first page footer of an Excel file.|
|get_first_page_footer(section)|Gets a script formatting the first page footer of an Excel file.|
|set_header_picture(section, header_picture)|Sets an image in the header of a worksheet.|
|set_footer_picture(section, footer_picture)|Sets an image in the footer of a worksheet.|
|set_picture(is_first, is_even, is_header, section, image_data)|Sets an image in the header/footer of a worksheet.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

