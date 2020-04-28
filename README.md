# Introduction

This is a Mechanical Turk template for tagging the meter of text from the Glossarial Concordance to Middle English,
https://middleenglish.library.jhu.edu/. The data is included as a spreadsheet.

# Usage

The template expects input of the following form:
```
"Identifier_0","Label_0","Text_0","Identifier_1","Label_1","Text_1","Identifier_2","Label_2","Text_2","Identifier_3","Label_3","Text_3","Identifier_4","Label_4","Text_4",
"01-1-ch.cat_01-1-ch_1","GP 1","Whan that Aprill with his shoures soote","01-1-ch.cat_01-1-ch_2","GP 2","The droghte of March hath perced to the roote,","01-1-ch.cat_01-1-ch_3","GP 3","And bathed every veyne in swich licour","01-1-ch.cat_01-1-ch_4","GP 4","Of which vertu engendred is the flour;","01-1-ch.cat_01-1-ch_5","GP 5","Whan Zephirus eek with his sweete breeth"
```

The identifier used is a combination of values that key into the original data available at https://github.com/jhu-digital-manuscripts/gcme.
It consists of the orginal file name, the file identifier provided for each line, and the line number separated by underscores. This allows reference back to the original data if needed. The label is the label of immediate work containing the line. The text consists of words separated by spaces. Punctuation may be attached to a word.

The output form maps each word to the stress status of its syllables. They key is the identifier from the input column plus the index of the word with a slash separator.

```
01-1-ch.cat_01-1-ch_6/0: uv
01-1-ch.cat_01-1-ch_6/1: vv
01-1-ch.cat_01-1-ch_6/2: uu
```

# Testing with ProtoTurk

Install ProtoTurk, https://github.com/hltcoe/prototurk.

```
prototurk task.html data.csv
```

Then visit http://localhost:8080/.
