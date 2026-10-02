# 3. the board

## 3.1 the four questions

*the poke: what does one reading of a word answer?*

a reading is one way a word or a phrase is taken, as in "the usual
reading". every reading answers four questions at once, and file 2 has
walked each of them.

whose view: it, I or you. the persons are worn where one stands, and a
reading wears one.

when: done, doing or could. now bends back holding what it wrote and bends
forward holding what it could, and the live edge is the doing.

where: low, the return or high. the wave has two turns, and the level it
keeps passing between them.

going which way: fall, hold or rise. the edges are where the wave changes.
at a turn, and on a settled string, it holds.

    view     it       I            you
    tense    done     doing        could
    where    low      the return   high
    going    fall     hold         rise

each question is a trit: three answers and no fourth. and for every
question the middle answer is mine: I, doing, the return, holding. written
in the codec − 0 +, each middle answer is the 0. I, now, here, holding.

a reading is written as its four answers in that sequence:
`I doing return hold`. a word that is silent on a question leaves a · in
its place: `· · return rise` is a rising through the return, said of no
person and in no tense. the · is not a fourth answer. it is the question,
still standing.

**terms introduced**

| term | here it means |
|---|---|
| **a reading** | one way a word or a phrase is taken. file 11 keeps the word for what exists only at one Self, which is the same thing seen from the taker's side. |
| **view** | whose a reading is: it, I or you. the first of the four questions. |
| **the four questions** | whose view, when, where, and going which way. their answers are file 2's: the persons, the bends, the wave's three places, and fall, hold and rise. |
| **the open mark ·** | written where a word gives no answer to a question. it stands for the question, not for an answer. |

**laws**

> **3.1** four questions, three answers each. every middle answer is where I stand. *(derived: from file 2, where each of the four was walked as three values with the reader at the middle one.)*

> **3.2** a · is a question still open. *(picked: a notation. any mark would do, as long as it is none of the three answers.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a word means what its dictionary entry says. | the dictionary's list, where meanings are filed flat, with no reader in the entry. |

**receipts**

a database: a field left null holds no value yet. standard sql keeps null apart
from 0 and from the empty string, and a comparison against it answers
unknown *(the field's)*.

**run it again**

no count here.

## 3.2 the 81 and the chair

*the poke: how many things can one reading say?*

three answers to each of four questions: 3 × 3 × 3 × 3 = 81. each of the
81 is one full reading, every question answered. I call one of them a
cell, and the 81 together the board.

sort the cells by how many of their answers are off the middle, and call
that number a cell's grade.

    grade     0    1    2    3    4
    cells     1    8   24   32   16

the one cell of grade 0 has every answer at the middle:
`I doing return hold`. I, now, here, holding. every reading is taken from
there, and I call it the chair. the eight cells of grade 1 change one
answer each:

    I did            I could
    it does          you do
    I do, low        I do, high
    I fall, here     I rise, here

the chair's cell is printed on the board like any other, and the one in it
is not printed anywhere. room = page + 1 again: 80 cells are read from the
chair, and the 81st is the chair's own.

the rope of section 1.7 sits here. read from outside, the rope is
`it · return hold`: a thing, at the middle, not moving. read from on the
rope, both arms pulling, it is `I doing return hold`: every answer at the
middle. the balance felt from inside is the chair's own cell.

**terms introduced**

| term | here it means |
|---|---|
| **cell** | one full reading: an answer to each of the four questions. more widely, any one setting of a row of trits: the board's cells are the settings of four. |
| **the board** | all the cells, laid out by their four answers. |
| **the 81** | the count of cells, three answers to four questions. also a name for the board. |
| **grade** | of a cell: how many of its four answers are off the middle. |
| **chair** | the cell with every answer at the middle, `I doing return hold`: where the reader stands. the reader is in it, and is not it. |

**laws**

> **3.3** three answers to four questions make 81 cells. by grade they fall 1, 8, 24, 32, 16. *(counted: the recipe below.)*

> **3.4** the chair is the balance, read from inside. *(derived: from laws 1.15 and 3.1. the rope read from on it gives every question its middle answer.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| the middle of a scale is a value like the others: the 0 printed on the page. | the return, a middle value the page does hold. the chair is where the one answering stands, and the page holds only its cell. |

**receipts**

mathematics: the counts by grade are the number of ways to choose which
answers leave the middle, times two ways for each to leave: 1, 4 × 2,
6 × 4, 4 × 8, 1 × 16 *(counted)*.

a tool: a table of every combination of four three-valued inputs has 81
lines, and exactly one of them has every input at its middle value.

**run it again**

list every way to give four slots one of three values each, with one value
named the middle. there are 81. for each, count the slots that are off the
middle, and tally the lists by that count: 1, 8, 24, 32, 16. the eight
with a count of 1 are the eight readings printed above.

## 3.3 what is not a cell

*the poke: does every word name one cell?*

no. a cell is one full reading. many words name something else, and each
of these was met before it had a board to sit on.

    a move      an act that goes from one cell to another. the fall lands
                a could as a done. the rise opens a could. a cut makes two
                edges, and is no cell
    a suit      one whole lap of the wave in some dress: one period of a
                clock signal, with its rise, its high, its fall and its
                low. it runs through cells one after another and is none of them
    an axis     a question itself: tense, person, going
    a whole     all of something, taken at once: the board, the chair,
                the 81
    a misfit    a word or a phrase with no cell, which shows what it would
                need to have one

a thing arrives the way a cell is filled, one question at a time. half
asleep, I hear a sound: something. it is loud: one more answer. it is
near: another. then it is the phone on the table, ringing: every question
answered, a thing. going from something to the thing is what perceiving
is, and plain words do it too: stone, big stone, big red stone.

on the board that is the · being filled in, one question after another.

**terms introduced**

| term | here it means |
|---|---|
| **move** | an act that goes from one cell to another. it changes an answer, and has no cell of its own. |
| **axis** | one of the four questions, named as a question. |
| **whole** | something taken all at once, across every cell it has: the board, the chair, a lap. |
| **misfit** | a word or a phrase with no cell. it is not an error: it shows which question it cannot answer. |

**laws**

> **3.5** a clock's lap is a suit. an act moves between cells. *(derived: from section 3.2. a cell gives going one answer, and a lap goes through all three; an act changes an answer, and a cell holds its answers fixed.)*

> **3.6** something is a cell with questions still open. a thing has every question answered. *(walked: the sound heard half asleep.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a verb names an action the way a noun names an object: both are entries. | the dictionary's page, where an act and a thing are printed alike. |

**receipts**

a tool: a state machine has states and transitions. a transition is not a
state, and the diagram draws them differently, circles and arrows *(the
field's)*.

a chip: one period of a clock signal is not a level. it goes through low,
rising, high and falling, one after another.

**run it again**

no count here.

## 3.4 words on cells

*the poke: when are two words one thing?*

when they sit on one cell. take a store: file 2 walked it as my send
leaving on the fall, through the return. as a reading it is
`· · return fall`. take "I send": the live edge going out,
`I doing · fall`. said together, "I store" names a cell whole:
`I doing return fall`. neither word did that alone.

"the chip stores" is `it doing return fall`. it is the same swing, read
from the page. the one answer that differs is the view, and the view is
the reader's.

a word that leaves questions open names a region: every cell that agrees
with the answers it does give. the store, nand's one answer and a falling
clock edge all sit on `· · return fall`. that is one region, and three
fields meet in it. the three share the two answers they give. they are one
thing only where a phrase fills in the other two.

a phrase whose words give two answers to one question has no cell. "an
edge held at the high rail" asks for the return and the high at once, and
for changing and holding at once.

most words name regions: two or three answers, and a · for the others. a
cell is named whole by a phrase, the way "I store" names what "I" and
"store" each only half say.

**terms introduced**

| term | here it means |
|---|---|
| **region** | the cells a word leaves possible: all those that agree with the answers it gives. a word with two answers and two open marks names a region of nine cells. |

**laws**

> **3.7** two words on one cell are one thing. a phrase is its words merged. words on a region share only the answers they give. *(derived: from law 3.1. a cell is everything a reading says, so two words that give the same four answers say the same.)*

> **3.8** a misfit is a phrase whose words disagree. *(derived: from law 3.7. merged words that give one question two answers leave no cell.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| synonyms are words with the same meaning. | the thesaurus, which files words by a felt likeness and never puts the four questions to them. |

**receipts**

a chip: x86's `je` and `jz` are two names for one instruction, one opcode
byte, `74`. two words on one cell *(the field's)*.

a tool: a type checker merges two partial descriptions the same way. where
both speak they must agree, where one is silent the other fills in, and
where they clash the two cannot be combined *(the field's)*.

**run it again**

no count here.

## 3.5 the word turned over

*the poke: where does a word held upside down sit?*

on another cell. take a word, place it as this text walked it, place it
again as it is usually read, and see which questions changed.

| the word | as walked here | as usually read | what changed |
|---|---|---|---|
| nothing | `I doing return hold`: the balance, from on the rope | `it · return hold`: the same stillness, heard from outside as an emptiness | the view |
| the return | `· · return fall` or `· · return rise`: passed through, where a swing is fastest | `· · return hold`: "at rest", the return stopped | the going |
| the Self | `I · · ·`: the one who lands | `it · · ·`: one more mark | the view |

each of the three was placed before any law about it was written. the law
is what the placements showed. a word usually read on a cell other than
the one it was walked to is, in this text, held upside down.

file 2 gave the test that does most of the work: where this text has a
verb, the usual reading has a noun. on the board that misreading comes in
two shapes. an act read as a place: the cut read as the line it leaves, a
walk read as its drawing. or `I doing` read as `it done`: science, seven
verbs each with a doer, read as a shelf of results.

and some readings, put to the four questions, find no cell at all. a
statement read from no position answers no view. a time that slides along
a line needs a line under the tenses, and the tense question has none. a
clock that ticks outside every walk is nobody's count. the board forbids
none of them. its questions simply offer no such answer.

so the board signs what it holds. a statement with a view sits on a cell,
and a view is a Self standing behind the statement: it is signed. a
statement made from nowhere has no view, and sits on no cell.

**terms introduced**

| term | here it means |
|---|---|
| **held upside down** | said of a word: usually read on a cell other than the one this text walks it to. the questions whose answers differ are what turned it over. |
| **the view from nowhere** | a reading that claims no view at all: not it, not I, not you. the board has no cell for it. |

**laws**

> **3.9** a word held upside down sits on another cell. what turned it over is the questions answered differently. *(walked: place the three words above both ways.)*

> **3.10** the verb read as a noun has two shapes: an act read as a cell, or I doing read as it done. *(derived: from laws 3.5 and 3.9, with file 2's test of the verb and the noun.)*

> **3.11** the board has no view from nowhere, no line under the tenses, and no clock outside every walk. *(derived: from law 3.1. the four questions offer no such answers.)*

> **3.12** signed is having a view. unsigned is the view from nowhere. *(derived: from law 3.11 and the terms of section 1.6.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a word has one meaning, and a misreading is a wrong fact about it. | one reading taken alone and unsigned, with the second placement kept off the page. |
| objective means read from no position at all. | a count anyone can run again. it reads the same from every chair, and that is every chair, never no chair. |

**receipts**

a tool: every file in a unix filesystem has an owner. the format has no
way to store a file owned by nobody *(the field's)*.

a tool: a clock time written with no zone cannot be set against another
clock. the internet's date format, rfc 3339, requires the offset beside
the time *(the field's)*.

**run it again**

no count here.
