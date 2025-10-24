##PageSetup class
## PageSetup class
Encapsulates the object that represents the page setup description.
The PageSetup object contains all page setup options.
The PageSetup type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [ods_page_background](/cells/python-net/aspose.cells/pagesetup/ods_page_background) | Gets the background of ODS. |
| [print_area](/cells/python-net/aspose.cells/pagesetup/print_area) | Represents the range to be printed. |
| [print_title_columns](/cells/python-net/aspose.cells/pagesetup/print_title_columns) | Represents the columns that contain the cells to be repeated on the left side of each page. |
| [print_title_rows](/cells/python-net/aspose.cells/pagesetup/print_title_rows) | Represents the rows that contain the cells to be repeated at the top of each page. |
| [black_and_white](/cells/python-net/aspose.cells/pagesetup/black_and_white) | Represents if elements of the document will be printed in black and white. |
| [center_horizontally](/cells/python-net/aspose.cells/pagesetup/center_horizontally) | Represent if the sheet is printed centered horizontally. |
| [center_vertically](/cells/python-net/aspose.cells/pagesetup/center_vertically) | Represent if the sheet is printed centered vertically. |
| [print_draft](/cells/python-net/aspose.cells/pagesetup/print_draft) | Represents if the sheet will be printed without graphics. |
| [footer_margin](/cells/python-net/aspose.cells/pagesetup/footer_margin) | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [footer_margin_inch](/cells/python-net/aspose.cells/pagesetup/footer_margin_inch) | Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [header_margin](/cells/python-net/aspose.cells/pagesetup/header_margin) | Represents the distance from the top of the page to the header, in unit of centimeters. |
| [header_margin_inch](/cells/python-net/aspose.cells/pagesetup/header_margin_inch) | Represents the distance from the top of the page to the header, in unit of inches. |
| [printer_settings](/cells/python-net/aspose.cells/pagesetup/printer_settings) | Gets and sets the settings of the default printer. |
| [left_margin](/cells/python-net/aspose.cells/pagesetup/left_margin) | Represents the size of the left margin, in unit of centimeters. |
| [left_margin_inch](/cells/python-net/aspose.cells/pagesetup/left_margin_inch) | Represents the size of the left margin, in unit of inches. |
| [right_margin](/cells/python-net/aspose.cells/pagesetup/right_margin) | Represents the size of the right margin, in unit of centimeters. |
| [right_margin_inch](/cells/python-net/aspose.cells/pagesetup/right_margin_inch) | Represents the size of the right margin, in unit of inches. |
| [top_margin](/cells/python-net/aspose.cells/pagesetup/top_margin) | Represents the size of the top margin, in unit of centimeters. |
| [top_margin_inch](/cells/python-net/aspose.cells/pagesetup/top_margin_inch) | Represents the size of the top margin, in unit of inches. |
| [bottom_margin](/cells/python-net/aspose.cells/pagesetup/bottom_margin) | Represents the size of the bottom margin, in unit of centimeters. |
| [bottom_margin_inch](/cells/python-net/aspose.cells/pagesetup/bottom_margin_inch) | Represents the size of the bottom margin, in unit of inches. |
| [first_page_number](/cells/python-net/aspose.cells/pagesetup/first_page_number) | Represents the first page number that will be used when this sheet is printed. |
| [fit_to_pages_tall](/cells/python-net/aspose.cells/pagesetup/fit_to_pages_tall) | Represents  the number of pages tall the worksheet will be scaled to when it's printed.
| [fit_to_pages_wide](/cells/python-net/aspose.cells/pagesetup/fit_to_pages_wide) | Represents the number of pages wide the worksheet will be scaled to when it's printed.
| [is_percent_scale](/cells/python-net/aspose.cells/pagesetup/is_percent_scale) | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [order](/cells/python-net/aspose.cells/pagesetup/order) | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
| [is_automatic_paper_size](/cells/python-net/aspose.cells/pagesetup/is_automatic_paper_size) | Indicates whether the paper size is automatic. |
| [paper_size](/cells/python-net/aspose.cells/pagesetup/paper_size) | Represents the size of the paper. |
| [paper_width](/cells/python-net/aspose.cells/pagesetup/paper_width) | Gets the width of the paper in unit of inches, considered page orientation. |
| [paper_height](/cells/python-net/aspose.cells/pagesetup/paper_height) | Gets the height of the paper in unit of inches , considered page orientation. |
| [orientation](/cells/python-net/aspose.cells/pagesetup/orientation) | Represents page print orientation. |
| [print_comments](/cells/python-net/aspose.cells/pagesetup/print_comments) | Represents the way comments are printed with the sheet. |
| [print_errors](/cells/python-net/aspose.cells/pagesetup/print_errors) | Specifies the type of print error displayed. |
| [print_headings](/cells/python-net/aspose.cells/pagesetup/print_headings) | Represents if row and column headings are printed with this page. |
| [print_gridlines](/cells/python-net/aspose.cells/pagesetup/print_gridlines) | Represents if cell gridlines are printed on the page. |
| [zoom](/cells/python-net/aspose.cells/pagesetup/zoom) | Represents the scaling factor in percent. It should be between 10 and 400. |
| [is_auto_first_page_number](/cells/python-net/aspose.cells/pagesetup/is_auto_first_page_number) | Indicates whether the first the page number is automatically assigned. |
| [print_quality](/cells/python-net/aspose.cells/pagesetup/print_quality) | Represents the print quality. |
| [print_copies](/cells/python-net/aspose.cells/pagesetup/print_copies) | Get and sets number of copies to print. |
| [is_hf_diff_odd_even](/cells/python-net/aspose.cells/pagesetup/is_hf_diff_odd_even) | True means that the header/footer of the odd pages is different with odd pages. |
| [is_hf_diff_first](/cells/python-net/aspose.cells/pagesetup/is_hf_diff_first) | True means that the header/footer of the first page is different with other pages. |
| [is_hf_scale_with_doc](/cells/python-net/aspose.cells/pagesetup/is_hf_scale_with_doc) | Indicates whether header and footer are scaled with document scaling.
| [is_hf_align_margins](/cells/python-net/aspose.cells/pagesetup/is_hf_align_margins) | Indicates whether header and footer margins are aligned with the page margins.
### Methods
| Method | Description |
| :- | :- |
| [`get_picture(self, is_header, section)`](/cells/python-net/aspose.cells/pagesetup/get_picture/#bool-int) | Gets the [`Picture`](/cells/python-net/aspose.cells.drawing/picture) object of the header / footer. |
| [`get_picture(self, is_first, is_even, is_header, section)`](/cells/python-net/aspose.cells/pagesetup/get_picture/#bool-bool-bool-int) | Gets the [`Picture`](/cells/python-net/aspose.cells.drawing/picture) object of the header / footer. |
| [`copy(self, source, copy_options)`](/cells/python-net/aspose.cells/pagesetup/copy/#aspose.cells.pagesetup-aspose.cells.copyoptions) | Copies the setting of the page setup. |
| [`set_fit_to_pages(self, wide, tall)`](/cells/python-net/aspose.cells/pagesetup/set_fit_to_pages/#int-int) | Sets the number of pages the worksheet will be scaled to when it's printed. |
| [`custom_paper_size(self, width, height)`](/cells/python-net/aspose.cells/pagesetup/custom_paper_size/#float-float) | Sets the custom paper size, in unit of inches. |
| [`clear_header_footer(self)`](/cells/python-net/aspose.cells/pagesetup/clear_header_footer/#) | Clears header and footer setting. |
| [`get_header(self, section)`](/cells/python-net/aspose.cells/pagesetup/get_header/#int) | Gets a script formatting the header of an Excel file. |
| [`get_commands(self, header_footer_script)`](/cells/python-net/aspose.cells/pagesetup/get_commands/#system.string) | Gets all commands of header or footer. |
| [`get_footer(self, section)`](/cells/python-net/aspose.cells/pagesetup/get_footer/#int) | Gets a script formatting the footer of an Excel file. |
| [`set_header(self, section, header_script)`](/cells/python-net/aspose.cells/pagesetup/set_header/#int-system.string) | Sets a script formatting the header of an Excel file. |
| [`set_footer(self, section, footer_script)`](/cells/python-net/aspose.cells/pagesetup/set_footer/#int-system.string) | Sets a script formatting the footer of an Excel file. |
| [`set_even_header(self, section, header_script)`](/cells/python-net/aspose.cells/pagesetup/set_even_header/#int-system.string) | Sets a script formatting the even page header of an Excel file.
| [`get_even_header(self, section)`](/cells/python-net/aspose.cells/pagesetup/get_even_header/#int) | Gets a script formatting the even header of an Excel file. |
| [`set_even_footer(self, section, footer_script)`](/cells/python-net/aspose.cells/pagesetup/set_even_footer/#int-system.string) | Sets a script formatting the even page footer of an Excel file.
| [`get_even_footer(self, section)`](/cells/python-net/aspose.cells/pagesetup/get_even_footer/#int) | Gets a script formatting the even footer of an Excel file. |
| [`set_first_page_header(self, section, header_script)`](/cells/python-net/aspose.cells/pagesetup/set_first_page_header/#int-system.string) | Sets a script formatting the first page header of an Excel file.
| [`get_first_page_header(self, section)`](/cells/python-net/aspose.cells/pagesetup/get_first_page_header/#int) | Gets a script formatting the first page header of an Excel file. |
| [`set_first_page_footer(self, section, footer_script)`](/cells/python-net/aspose.cells/pagesetup/set_first_page_footer/#int-system.string) | Sets a script formatting the first page footer of an Excel file. |
| [`get_first_page_footer(self, section)`](/cells/python-net/aspose.cells/pagesetup/get_first_page_footer/#int) | Gets a script formatting the first page footer of an Excel file. |
| [`set_header_picture(self, section, header_picture)`](/cells/python-net/aspose.cells/pagesetup/set_header_picture/#int-bytes) | Sets an image in the header of a worksheet. |
| [`set_footer_picture(self, section, footer_picture)`](/cells/python-net/aspose.cells/pagesetup/set_footer_picture/#int-bytes) | Sets an image in the footer of a worksheet. |
| [`set_picture(self, is_first, is_even, is_header, section, image_data)`](/cells/python-net/aspose.cells/pagesetup/set_picture/#bool-bool-bool-int-bytes) | Sets an image in the header/footer of a worksheet. |
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
sheets = workbook.worksheets
# Add a worksheet
sheets.add()
sheet = sheets[1]
pageSetup = sheet.page_setup
pageSetup.print_area = "D1:K13"
```
### See Also
* module [`aspose.cells`](..)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)
