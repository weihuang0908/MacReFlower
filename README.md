![Icon](https://raw.github.com/fibasile/MacReFlower/master/icon.iconset/icon_256x256.png ) 

MacReFlower
===========

ORIGIN PROJECT:https://github.com/fibasile/MacReFlower

This is a little utility app that allows to drop PDF files and get them optimized for viewing on the Kindle Paperwhite, but
might work for other e-Ink devices..

The program uses the [k2pdfopt](http://www.willus.com/k2pdfopt) utility, which you should download and put in your PATH,
i.e. in /usr/local/bin folder.

**Please also make sure that k2pdfopt is executable (i.e. chmod +x k2pdfopt)**

Default k2pdfopt options are in MacReFlower/MRFAppDelegate.m 

//$k2pdfopt -o a.pdf L3\ mapreduce-osdi04.pdf -dev kpw -mode 2col -ws 0.375 -ls- -ui-
- (void)runConversionTask:(id)sender {
    NSArray* defaultOptions = [NSArray arrayWithObjects:
                               @"-dev",
                               @"kpw",
                               @"-mode",
                               @"2col",
                               @"-ws",
                               @"0.375",
                               @"-ls-",
                               @"-ui-",
                               @"-x",
                               nil];

Users can alter these options as needed.


Screenshots
===========
![Initial screen](https://raw.github.com/fibasile/MacReFlower/master/screenshots/screenshot.png)
![Conversion progress](https://raw.github.com/fibasile/MacReFlower/master/screenshots/screenshot2.png)



License
=======

MacReFlower is distributed under the MIT License. See the LICENSE.txt for more information.


Contact information
==================

Fiore Basile

github: fibasile.github.io
twitter: @fibasile
email: <fiore.basile@gmail.com>
