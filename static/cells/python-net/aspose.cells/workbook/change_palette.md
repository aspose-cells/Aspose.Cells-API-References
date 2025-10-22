##change_palette method
## change_palette(self, color, index) {#aspose.pydrawing.Color-int}
Changes the palette for the spreadsheet in the specified index.
```python
def change_palette(self, color, index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| color | aspose.pydrawing.Color | Color structure. |
| index | int | Palette index, 0 - 55. |
### Remarks
The palette has 56 entries, each represented by an RGB value.
If you set a color which is not in the palette, it will not take effect.
So if you want to set a custom color, please change the palette at first.
The following is the standard color palette.
| Color | Red | Green | Blue |
| :- | :- | :- | :- |
| Black| 0| 0| 0 |
| White| 255| 255| 255 |
| Red| 255| 0| 0 |
| Lime| 0| 255| 0 |
| Blue| 0| 0| 255 |
| Yellow| 255| 255| 0 |
| Magenta| 255| 0| 255 |
| Cyan| 0| 255| 255 |
| Maroon| 128| 0| 0 |
| Green| 0| 128| 0 |
| Navy| 0| 0| 128 |
| Olive| 128| 128| 0 |
| Purple| 128| 0| 128 |
| Teal| 0| 128| 128 |
| Silver| 192| 192| 192 |
| Gray| 128| 128| 128 |
| Color17| 153| 153| 255 |
| Color18| 153| 51| 102 |
| Color19| 255| 255| 204 |
| Color20| 204| 255| 255 |
| Color21| 102| 0| 102 |
| Color22| 255| 128| 128 |
| Color23| 0| 102| 204 |
| Color24| 204| 204| 255 |
| Color25| 0| 0| 128 |
| Color26| 255| 0| 255 |
| Color27| 255| 255| 0 |
| Color28| 0| 255| 255 |
| Color29| 128| 0| 128 |
| Color30| 128| 0| 0 |
| Color31| 0| 128| 128 |
| Color32| 0| 0| 255 |
| Color33| 0| 204| 255 |
| Color34| 204| 255| 255 |
| Color35| 204| 255| 204 |
| Color36| 255| 255| 153 |
| Color37| 153| 204| 255 |
| Color38| 255| 153| 204 |
| Color39| 204| 153| 255 |
| Color40| 255| 204| 153 |
| Color41| 51| 102| 255 |
| Color42| 51| 204| 204 |
| Color43| 153| 204| 0 |
| Color44| 255| 204| 0 |
| Color45| 255| 153| 0 |
| Color46| 255| 102| 0 |
| Color47| 102| 102| 153 |
| Color48| 150| 150| 150 |
| Color49| 0| 51| 102 |
| Color50| 51| 153| 102 |
| Color51| 0| 51| 0 |
| Color52| 51| 51| 0 |
| Color53| 153| 51| 0 |
| Color54| 153| 51| 102 |
| Color55| 51| 51| 153 |
| Color56| 51| 51| 51 |
### See Also
* module [`aspose.cells`](../../)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
