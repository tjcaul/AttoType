# AttoType

## Intended Usage

I designed these fonts for use in pixel art and low-resolution displays (like a 128x64 GLCD).
I have not created any OpenType (or similar) font files, since these fonts are not intended
to be used on systems where such fonts are available.

## Rationale

The 3x4 and 3x5 fonts each come in only one variant, where every character is unique.

The 3x3 font has three variants: uppercase, lowercase, and unique.

In the uppercase font, all letters are uppercase.
This is great for displaying text, as it's (somewhat) readable.

The lowercase font distinguishes between uppercase and lowercase where possible.
The lowercase letters aren't all the same height, and don't have descenders, making them look odd.
In an application where capitalization matters, this is the way to go.

In these two variants, some characters are identical (like `$`, `5`, and `S`).
In context, it should be clear which character is being used.
However, consider the case of a terminal or code editor, where every character has a special meaning,
and numbers are often mixed with letters.
The unique font is designed for this purpose.
Some glyphs are not intuitive, like `2`, `5`, `f`, and `k`.
It's an unfortunate tradeoff between legibility and accuracy.

## Background

When considering making a web browser for the Arduino Uno + ESP8266, I knew I needed a small
font for my 320x240 TFT touchscreen. As I couldn't find any small fonts that strictly followed
size rules and had the whole ASCII character set, I decided to make one (or five) myself.


