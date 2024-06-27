---
Test Memo using ESCMarkdown

AUTHOR: Brendan Arndt

RECIPIENT: Me
RECIPIENT: Myself
RECIPIENT: I

DATE: TODAY
---

TABLE OF CONTENTS

LIST OF FIGURES

LIST OF TABLES

# 1. Fun Formatting Options #[Section-1]


Surrounding text with...

One asterisk (\*) or underscore (\_) can *make text italicized!*

Two asterisks (\*\*) or underscores (\_\_) can **make text bold!**

Three asterisks (\*\*\*) or underscores (\_\_\_) can 
***make text bold and italicized!***

One backtick (\`) can `make text monospace!`

Using the caret symbol (\^) and curly braces can make super^{script}

Using the underscore (\_) and curly braces can make sub_{script}

The line about the bold and italicized text (and this one) went over 
the 80 character limit so it had to be split into two lines!

# 1. Creating Figures and Tables? #[Section-2]


## 1.1 Figures #[Section-2-1]


Each Figure can get a Title, Tag, Legend, Scale, and Image

FIGURE 1.: Big Cat Picture I Stole from Wikipedia

The scale is set to 5!

SCALE [5][Cat03.jpg]

FIGURE 2.: Small Cat Picture I Stole from Wikipedia

The scale is set to 1!

SCALE [1][Cat03.jpg]

The scale of a Figure can be anywhere from 10 - 100\% of the page!

This is done using the SCALE feature, which takes a number from 1-10,
multiplies it by 10, then uses that as the \% of space the Figure should
take up on the page!


In the examples above...

the Titles were \"(Big/Small) Cat Picture I Stole from Wikipedia\"

the Tags cannot be seen, but are \"big-cat\" and \"small-cat\"

the Legends were \"The scale is set to (10/3)\"

the Scales were \"100\%\" and \"30\%\"

the Image was the same cat between both Figures

The code for Figure 1 can be found in REF[FIG1].

The code for Figure 2 can be found in REF[FIG2].

## 1.1 Tables #[Section-2-2]

Tables can be constructed and represented in a similar way to Figures.

TABLE 1.: Example Table #[my-table] NO-EXTERNALIZE

Tables can have Legends too!

-----
column_1 | column_2 | column_3
@Type string | @Type string | @Type string
-----
value_1 | value_2 | value_3
value_4 | value_5 | value_6
value_7 | value_8 | value_9
-----

Entries can be delimitted using the pipe operator (|) or commas (,).

Each Line represents a Row.

A Header can be included by seperating the first row using a dashed line.

Just like Figures, Tables also have a Title, Tag, and Legend


In the above Table...

the Title is \"Example Table\"

the Tag (unseen) is \"my-table\"

the Legend is \"Tables can have Legends too!\"

The code for this Table can be found in REF[TAB1].

# 1. Mathematical Functions and Symbols #[Section-3]


Mathematical functions and symbols can be demonstrated using
a single dollar sign ($) at the start and end of the line
or three dollar signs at the start and end of a block of text.

For example,

$ \\sqrt{25} = 5 $

$ 800.2 \\approx 800.0 $

$ \\frac{45}{50}=0.9 $


This is done using commands and syntax from LaTeX.

# 1. Using Verbatim Text #[Section-4]


Using three backticks (```) across two lines of allows the
block of text within to be ignored.
This lets leading and trailing whitespace persist.

For example,
```
    This   Text   Is   Being
    Read     Back   Verbatim,
 Spacing         Errors      And    All      !
```

# 1. Numbered and Non-Numbered Lists #[Section-5]


1. Lists can be made using bullet points or with numbers
1. This list uses numbers
1. But the system handles the counting for us
    50. In fact, the first set in this list was written with all \"1.\"s
    49. This part is weird too
    48. The numbering on my end is backwards!
        47. Better yet, I started from 50!
1. Lists are based on indentation, just like Microsoft Word


* Asterisks can be used to make bullet points
- Hyphens can also be used
+ Plus can be used too!
    * Just make sure that lists are seperated by at least 2 blank lines
    * If not, the formatting will persist!
        - This can be useful for inserting a paragraph between items in a list!

===
===

# Markdown Code for Figures

## Figure 1 #[FIG1]
```
FIGURE 1.: Big Cat Picture I Stole from Wikipedia

The scale is set to 5!

SCALE [5][Cat03.jpg]
```

## Figure 2 #[FIG2]

```
FIGURE 2.: Small Cat Picture I Stole from Wikipedia

The scale is set to 1!

SCALE [1][Cat03.jpg]
```

# Markdown Code for Tables

## Table 1 #[TAB1]

```
TABLE 1.: Example Table #[my-table] NO-EXTERNALIZE

Tables can have Legends too!

-----
column_1 | column_2 | column_3
@Type string | @Type string | @Type string
-----
value_1 | value_2 | value_3
value_4 | value_5 | value_6
value_7 | value_8 | value_9
-----
```

