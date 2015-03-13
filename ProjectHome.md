This is very simple implementation of the Excel 97-2003 format written in C++. This library was deveoped only for reading Excel files, so you can't write Excel file with this library.

Please visit [Home Page](http://igor-mironchik.besaba.com/projects/readexcel.html).

# Example #

```
Excel::Book book( L"sample.xls" );

Excel::Sheet * sheet = book.sheet( 0 );

std::wstring cel0 = sheet->cell( 0, 0 ).getString();
double cel1 = sheet->cell( 1, 1 ).getDouble();
double cel3 sheet->cell( 3, 1 ).getFormula().getDouble();
```