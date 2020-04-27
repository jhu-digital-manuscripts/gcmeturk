# Introduction

This is a Mechanical Turk template for tagging the meter of text from the Glossarial Concordance to MIddle English,
https://middleenglish.library.jhu.edu/.

# Usage

The input...


```
"Identifier_0","Label_0","Text_0","Identifier_1","Label_1","Text_1","Identifier_2","Label_2","Text_2","Identifier_3","Label_3","Text_3","Identifier_4","Label_4","Text_4",
"01-1-ch.cat_01-1-ch_1","GP 1","Whan that Aprill with his shoures soote","01-1-ch.cat_01-1-ch_2","GP 2","The droghte of March hath perced to the roote,","01-1-ch.cat_01-1-ch_3","GP 3","And bathed every veyne in swich licour","01-1-ch.cat_01-1-ch_4","GP 4","Of which vertu engendred is the flour;","01-1-ch.cat_01-1-ch_5","GP 5","Whan Zephirus eek with his sweete breeth"
```


This can be tested using prototurk.


The output...

```
01-1-ch.cat_01-1-ch_6/0: uv
01-1-ch.cat_01-1-ch_6/1: vv
01-1-ch.cat_01-1-ch_6/2: uu
```