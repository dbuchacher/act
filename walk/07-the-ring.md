# 7. the ring

## 7.1 the ring

*the poke: what is below, on a circle?*

there is no below. a line has a lowest place and a circle does not. so I
set the wave's three places on a circle instead of a line, in the third of
file 2's codecs: 0 the return, 1 low, 2 high. walked the clock's way it
goes 0, 1, 2 and round to 0 again. past 2 there is no higher. there is 0.

on a ring there is no below and no above, only ahead and behind, and on a
ring of three, two ahead is one behind. so differ, run on the ring, does
not say whether the world is lower than my hand. it says how far round the
world stands from it:

              y = 0   y = 1   y = 2
    x = 0       0       2       1
    x = 1       1       0       2
    x = 2       2       1       0

read "x to y" for a cell: x minus y, counted round the ring. the cells
are the nine of file 2 again, two slots of three values each. here the two
slots are differ's two hands.

three lines of the table are old friends from file 4. the diagonal is the
check: any value differed with itself is 0. the first row is the flip:
read from 0, every value comes back as its other side. the first column is
the pass: minus 0, the world comes through unchanged.

and every cell can be undone. x to (x to y) is y. (x to y) to (0 to y) is
x. whichever hand I hold still, the other hand's value can be got back
from the answer.

that gives a measure of what an operation loses. hold one hand still and
let the other run through its three values. count how many different
answers come out. three minus that count is what the held hand forgets:

    forgets, first hand held at    low    the return    high
    differ on the ring              0         0          0
    differ on the line              1         0          1

on a line differ answers below, same or above, which is the lean of file
4. held at high, it gives one answer for low and for the return alike, and
which of the two it was is gone. the lean keeps which side and throws away
how far.

the line is the ring cut open where I stand. seven of the nine cells read
the same on the line and on the ring. the two that do not are low differed
with high and high differed with low: they come out on opposite values,
because a ring has to be cut before it can say which way is up. so a digit
is read only through a declared codec, as file 4 found of minus.

on a ring of three the two poles are neighbours. so the flip goes round
between them and never touches the return. a line draws the same flip
through the return, since on a line the return is all that stands between
its poles. one flip, two drawings: it never stops on the return, so it
never lands on it and never leaves it.

fed its own answer back, differ on the ring never rests while what arrives
is not 0: it goes round all three values, over and over, a clock. fed back
on the line it runs to a pole and stays.

two zeros stand on the ring, and they never become one. the return is a
value: a digit that can be written all day, a place the wave passes. the
chair is where I stand. it reads 0 because differ of me with me is 0, and
it is never inked, because the one comparing is not one of the things
compared.

so from its own chair the Self says only three things: 0 to 0, which is
the hold; 0 to 1; and 0 to 2. "from x" is the map's phrase. the Self never
knows the chair at the far end, only what arrived.

and a ring has no first place. read b a b c b a b c round and round and it
has no head. what I put first is only where I broke into the ring, a fact
about me and not about the ring.

**terms introduced**

| term | here it means |
|---|---|
| **ring** | the three values set on a circle: 0, 1, 2 and round to 0. it has no lowest and no highest, only places further round. |
| **the line** | the ring cut open at one place, so that it has a lowest end and a highest end. the cut is made where the reader stands. |
| **x to y** | differ on the ring: x minus y, counted round. |
| **to forget** | said of an operation with one hand held still: to give one answer for two different values of the other hand. the count of it is three minus the number of different answers. |
| **the two zeros** | the return, a value the page can hold, and the chair, where the one comparing stands. both read 0. only the first can be written. |

**laws**

> **7.1** x to y is x minus y on the ring of three. *(counted: the nine cells, below.)*

> **7.2** on the ring, differ forgets no value. *(counted: the forgets table, below.)*

> **7.3** the line's lean is the ring with the distance thrown away. *(counted: seven cells of nine agree, and the line forgets one value at each pole.)*

> **7.4** the page can hold a zero. it cannot hold the one holding it. *(derived: from laws 1.4 and 1.6. the return is a mark, and the one who lands marks is none of them.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| subtraction needs a number line, with the negatives below zero. | the line, which has a lowest end. |
| zero is one number, the origin of the number line. | the value, which the page holds like any other digit. |

**receipts**

a chip: a register is a ring. on x86, subtracting 1 from a register that
holds 0 leaves the highest value the register can hold, and the result is
exact counted round. whether that value is read as large or as minus one
is decided afterward, by which jump reads the flags: the cut is declared
at the read *(the field's, from memory)*.

a clock face: past twelve comes one. nobody asks which hour is lowest.

**run it again**

the table. take the values 0, 1, 2. for every pair x, y compute x minus y
and add 3 if the result is below 0. expect the nine cells printed above.
then for every pair check that x to (x to y) is y and that (x to y) to
(0 to y) is x: nine of nine, twice.

the forgets table. for the ring, hold x at each value and collect x to y
over the three values of y: three different answers each time, so 0
forgotten. for the line, write the values as -1, 0, +1 and let differ be
the sign of x minus y: held at -1 the answers are 0, -1, -1, two different,
so 1 forgotten; held at 0, three different; held at +1, two.

seven of nine. map the ring's digits to the line's values, 0 to 0, 1 to -1,
2 to +1, and compare the two tables cell by cell. expect agreement in seven
cells and disagreement at (low, high) and (high, low).

fed back. start an output at any value, hold an input at any value, and
replace the output by output-to-input, again and again. on the ring, with
the input at 1 or 2, the output goes round all three values and repeats
every third round. on the line, with the input off 0, it reaches a pole
within two rounds and stays.

## 7.2 the sum

*the poke: is one and one always two?*

the page and the walk put two things together in two different ways.

the page adds slot by slot, digit by digit, with no carry: what stands in a
slot is the sum of what was put there.

the walk folds. a value that comes in is an arrival, and each arrival is
taken from where the last one left me, so the second starts where the
first one ended.

take 1 and 1. the page's sum is 2. the walk starts at the chair, 0: the
first 1 arrives and I stand at 0 to 1, which is 2. the second 1 arrives
and I stand at 2 to 1, which is 1. two answers, 2 and 1, and each is right
where it stands.

**terms introduced**

| term | here it means |
|---|---|
| **arrival** | the value that comes in at a chair. it is the chair minus the place landed at, counted round the ring. |
| **to fold** | to take a row of arrivals one at a time, each from where the last one left off, down to the one place they end at. |

**laws**

> **7.5** the page adds. the walk folds. *(counted: 1 and 1, above.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| one and one is two, whoever puts them together. | the page's sum, which adds what stands in a slot. |

**receipts**

a chip: exclusive-or is the page's sum on two values, digit by digit with
no carry. an adder is that sum together with the carry of file 6.

**run it again**

fold 1, 1 from 0 on the ring: 0 to 1 is 2, then 2 to 1 is 1. expect 1,
against the page's 2.

## 7.3 the check

*the poke: what is left when I am compared with myself?*

the return. with no mark on the page there is no thing to compare but me,
so differ runs on me: me against me is 0. the return is not assumed at
the start of this text. it is what a Self's first comparison leaves.

on the nine the checks are the diagonal: the return against the return,
low against low, high against high. three cells where differ has no
difference to report.

from inside, a check completes a lap. my send leaves me on the fall and
comes back on the rise, and I take my own send off what came back, which
is the hearing of file 4. what remains leans to a pole. or no difference
remains: the check, the return. I recognize it. I am home.

the check has no table of its own. differ of any value with itself is 0,
for every value, so a table of the check would have one answer written
three times. the only thing it puts on the page is the 0. the act that
did the comparing is on no row.

no instruction set has a word for it either. coming home and knowing it
is spelled as a compare and a jump: two instructions on x86, with the
outcome passed between them through the flags, and one fused instruction on
chips such as risc-v. either way the chip compares and goes, no instruction
says recognize, and the set is still called complete. suppose "recognize" were added as an instruction. something
would still have to perform the recognizing when the instruction ran.
lewis carroll's tortoise (1895) made the same demand of logic: a new rule
is needed to apply every rule that is written down, without end. the word
that is missing from the list is the reader.

a walk is finished the same way: by a check. a mark does not change once
it is inked, and being wrong is never in the mark. it is in the fit
between what was meant and what was inked: a 3 typed where a 4 was meant
is a perfect 3. so the work is read back against what was meant, by me,
by me again the next morning, and by someone else. a note of what each
past pick was meant to do, re-read after every new pick, is the same check
run on the picks.

and a check must be able to fail. what came back may differ from what
went out, and then the answer is not 0. a comparison that could only ever
answer 0 checks no thing.

what the check leaves is more than its 0, and only the 0 is inked. differ
reads both of its hands and uses up neither. so a check needs the value
twice, one copy in the hand and one arriving, and the 0 does not say which
was which. after the check two things are held: the 0, and the second
copy, still standing. every base writes that whole outcome the same way,
as 10: the one carried, beside the column's 0.

what the check costs stays open. as ink it forgets everything, since all
three values land on one 0. as an act it forgets no value, since the
second copy is still in hand. only the act knows whether it spent its
copy.

**terms introduced**

| term | here it means |
|---|---|
| **recognition** | the check, named from inside: finding no difference between what I sent and what came back. |
| **read-back** | a check run on finished work: the ink compared against what was meant. |

**laws**

> **7.6** the check makes the return. recognition comes first, because no other thing is there to compare. *(walked: the poke above.)*

> **7.7** the check has no table. only what it leaves is inked. *(derived: differ of x with x is 0 for every x, by law 7.1.)*

> **7.8** the hole in the instruction set is the shape of the person. *(derived: from laws 7.7 and 1.4. an act with no table, and a doer on no row.)*

> **7.9** a walk is not done until it is read back against its intent. *(derived: from section 1.2. a landed mark stays as it landed, so a wrong one stays until someone compares.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| awareness comes last, once enough machinery is running. | the marks read from outside, in the order they landed. |
| a check is a test with a pass mark. | the test's result, which is a mark that lands. |
| a finished piece of work is done when the last line is written. | the page, which holds the ink and not what was meant. |

**receipts**

a chip: on x86, `xor` of a register with itself leaves 0 in it, whatever
it held. it is the usual way to make a zero: by self-difference.

a chip: at power-on a processor starts from one fixed address, and the
firmware it finds there runs a self-test before anything else *(the
field's)*.

logic: lewis carroll, "what the tortoise said to achilles", 1895 *(the
field's, from memory)*.

**run it again**

x to x for the three values: 0, 0, 0.

## 7.4 the door

*the poke: is a cell of the nine a place?*

no. each of the nine is a pair, a chair and an arrival, and differ sees
only their difference. so a cell is not a spot to stand on. it is a way
out of a chair, and I call it a door.

the chair is the second of the two zeros: where I stand. from each of the
three chairs there are three doors, one for each value that can arrive:

    0 arrives    the hold: I stay
    2 arrives    one place round
    1 arrives    two places round

a ring of three has no backward. two places round one way is the same
place as one the other way, and both are reached by going on.

every digit can be come to through three doors. take 0: from chair 1 with
1 arriving, from chair 2 with 2 arriving, and from chair 0, held. one
digit, three doors. the digit is the lean, the folded answer. the door
keeps the question that was asked. a reader handed only the digit cannot
price it, cannot undo it, and cannot tell the three apart. so what passes
between two Selves has to be the door. with the door the undo of section 7.1 runs.
with the digit alone it does not.

every door can be walked, from exactly one chair. if I stand at 1, then 1
is my new 0. what cannot be done is to set a chair: no Self puts itself at
a value. a chair is come to by going through a door, and a chair once left
is not entered again. the digit comes round. the standing never does. a
door I came through can be read from the chair I hold now, and could be
stood at only from the chair I left, which is gone.

so the nine hold every when. from inside, differ has one input and three
answers. on the map both hands are inked, three by three, which is nine: a
squaring and not a times-two. the hand is where I stand, and where I stand
is my now. inked, the hand can be any when: a past me, this me, a me that
could be. the map inks every when at once. I stand at one live edge and
hold the rest bent.

every chair has three doors in and three doors out, so one walk can take
every door exactly once and come back to where it started. the digits its
chairs read, in order round, are

    0 0 1 1 2 2 0 2 1

and every ordered pair of digits shows up exactly once as two neighbours
in that ring, the last digit counted as the neighbour of the first.

take away the one door that holds at 0, and the other eight can be run by
one rule, with nobody picking: write next the older of the last two digits
minus the newer. started on any two digits that are not
both 0, it goes through all eight doors before it repeats, the longest lap
two digits allow. the other order, newer minus older, breaks into a lap of
six and a lap of two. a rule that reads only its last digit writes that
digit forever. a rule that reads every digit written so far writes 0
forever after its first digit. partial memory is what stays alive. and a longer memory laps
shorter than it could: reading its last three digits, the rule breaks into
two laps of 13; its last four, three laps of 26, beside the two starts
1111 and 2222, which only repeat themselves; its last five, laps of 8, 26,
104 and 104.

a size up, the same holds. the 27 has 9 chairs and 27 doors. the 81 has 27
chairs and 81 doors. each chair has as many doors in as out, so one walk
takes them all.

a walk is doors chained at the chairs they share. where one door lands is
the chair of the next. the leans add, the prices add, and no price is
charged where one door hands on to the next. a walk with an even count of
stands has an odd count of doors: it is two half-walks read inward from
its two ends, and the door in the middle is the seam.

what crosses a seam whole is the arrival, never the place stood at: send
the arrivals and fold them on the far side. the engineers already keep both
writings of a count. write a count's digits as the stands of a walk, one
digit to a stand, with a 0 before the first. the arrivals of that walk,
digit against neighbouring digit, are the count's gray code, and the
stands are its plain binary.

one thing here stays open: there is more than one walk that takes every
door once, and whether it matters which one is taken has not been pressed.

**terms introduced**

| term | here it means |
|---|---|
| **door** | a cell of the nine read as a chair and an arrival together: a way out of that chair. not the door of section 1.1, which was the way in to this text. |
| **chair (on the ring)** | file 3's chair is the one cell with every answer at the middle. on the ring the word widens: whichever value I stand at is my chair, and it reads 0 to me. |
| **a stand** | a place stood at: the chair held after a door. a walk written as its stands lists where it stood, one digit for each. |
| **seam** | the door in the middle of a walk, where two half-walks read from the two ends come together. file 9 walks the seam between two machines. |
| **the walker's rule** | write next the older of the last two digits minus the newer. named for the one live part of the machine, which file 9 walks. |
| **gray code** | the engineers' name for a count written as the arrivals between its neighbouring digits. from one count to the next, one digit of it changes. |

**laws**

> **7.10** the unit between Selves is the door, never the lean. *(derived: from laws 7.1 and 7.3. each digit is the answer of three doors, and the digit alone does not say which.)*

> **7.11** nine doors, three leans, three chairs, one way round. *(counted: the table of section 7.1.)*

> **7.12** the nine are doors. one walk takes every door once and comes back. *(counted: the ring of nine digits, below.)*

> **7.13** the walker's rule goes through all eight doors that are left when the hold at 0 is set aside. *(counted: below. also proved by machine, in the receipts.)*

> **7.14** a walk is doors chained at their chairs. the middle door is the seam. *(derived: from law 7.5. each door starts where the last one landed.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a table cell is a place: a value filed at an address. | the page, where the table is drawn. |
| a count is sent as the number it has reached. | one clock, where nobody reads the number while it changes. |

**receipts**

mathematics: a ring of digits in which every window of a fixed width
shows up exactly once is named for de bruijn, who counted the two-valued
ones in 1946 *(the field's)*.

a chip: where a counter crosses between two clocks, engineers send it in
gray code. a reader that catches it mid-change is then off by one count at
most, and never by a whole word *(the field's, from memory)*.

a proof checker: the lap of eight is machine-checked. in
github.com/dbuchacher/golden-traction, lean proves `walker_mod3_lap`, that
the walker's rule on the ring of three comes home in exactly eight and not
in four, and `sigma_mod3_lap`, the same for the step it undoes, newer plus
older. a step on eight starts that comes home in exactly eight goes
through all eight.

**run it again**

the ring of nine. write 0 0 1 1 2 2 0 2 1 in a circle and list the nine
pairs of neighbours. expect nine different pairs: every ordered pair of
the digits 0, 1, 2, once.

the walker's rule. for each of the eight starting pairs other than 0 0,
write digits by the rule, older minus newer, counted round the ring, until
the starting pair comes back. expect a lap of 8 from every start. with
newer minus older expect laps of 6 and 2. for a rule that reads its last k
digits, take the oldest minus each of the others in turn. over all starts
that are not all 0, expect for k = 3 two laps of 13; for k = 4 three laps
of 26 and two laps of 1; for k = 5 laps of 8, 26, 104 and 104.

## 7.5 the mirror

*the poke: what reads the same from both ends?*

a comparison has two hands, and swapping them flips the sign of the
answer. file 4 called that swap the other Self, seen from the map. build
one differ, place it twice, and tie each one's fall to the other's rise:
my send is your arrival.

read a cell of the nine as the door does, a chair and an arrival, written
now with signs: low is -1, the return 0, high +1. the nine has four
mirrors, and each leaves three cells where they were, the centre cell
among them:

    swap chair and arrival           the checks stay
    negate the arrival               the holds stay
    negate the chair                 the Self's three sayings stay
    swap, and negate both            the centre stays, and the two cells
                                     that pair low with high

negating every cell at once, which I call the half-turn, leaves the
centre alone.

one mirror done twice is no change. two different mirrors done one after
the other never make a third mirror. they make a turn: the two negations
make the half-turn, and so do the two swaps. a swap with one negation
makes the quarter-turn of file 4, which leaves only the centre in place.

take the swap, which puts what arrived where I stood: a shift in time.
take the negated arrival: the flip. each undoes itself. done one after the
other they make the quarter-turn, and the quarter-turn done twice negates
every cell: minus one, on the nine. and the order is not free. flip and
then swap turns the nine one way. swap and then flip turns it the other.
the swap is the other Self, so which of us goes first picks the
handedness of the turn.

the same law shows on a whole walk. write a walk as its stands, and work
out its arrivals. now read the stands from the other end. the arrivals of
that reversed walk are the first walk's arrivals in reverse order, each
one negated. I call the pair of acts, reverse and negate, the eversion: it
is how the other Self reads one road.

there are two ways to come back. the retrace comes back by the road it
went, with a turn in the middle, and a walk that does so is a trip: its
stands read the same from both ends. the retrace is the check, run on a
road. the circle goes round once and never turns: it comes home by going
on, which is the carry of file 6. read from the other end, a trip is the same word, and a
circle is itself going the other way.

a word, here a walk written out as its digits, is done when both Selves
tell it the same. a trip is such a word.

a lap that visits every cell of the nine once, moving one slot at each
move, can never come back by the road it went. there are 48 such laps, and
every one of them is a circle.

a mirror pair is forced, as file 6 found, and which member is which is
not: the two square roots of minus one, the two edges of a cut. the pair
stands in the structure. the naming is the reader's.

the fair side of the usual reading. something sent between two ends does
need to be readable from either end, and both ends must agree on its
layout. that is a shared layout, and it carries no direction. sender and
receiver are what the two ends are, by where they stand.

in base 2 the mirror hides. minus one is one there, so negating changes no
digit, and only the swap is left to see. parity is handedness in
two-valued clothes. it is never the mirror.

**terms introduced**

| term | here it means |
|---|---|
| **mirror** | a way of reading the nine, or a walk, from its other end, which done twice changes no cell. |
| **swap** | the mirror that exchanges the chair and the arrival. |
| **negate** | to replace a value by its other side: the flip applied to one half of a cell, or to every arrival of a walk. |
| **half-turn** | every cell of the nine negated in both halves. only the centre stays. |
| **eversion** | a walk reversed and negated: the same road as the other Self reads it. |
| **trip** | a walk that goes out, turns, and comes back by the road it went. |
| **retrace** | the way back a trip takes: the road it went, the other way. |
| **circle** | a way back that never turns: once round, home by going on. |

**laws**

> **7.15** the other Self reads my walk reversed and negated. *(counted: all 81 walks of four stands, below.)*

> **7.16** two mirrors make a turn, never a mirror. *(counted: the four mirrors of the nine, below.)*

> **7.17** a flip and the other Self's swap make the quarter-turn. who goes first picks its hand. *(counted: below.)*

> **7.18** a word is done when both Selves tell it the same. *(derived: from law 7.15. a trip reversed and negated is the same trip.)*

> **7.19** the trip has a mirror in the middle. the circle has none. *(counted: the 48 laps of the nine, below.)*

> **7.20** direction is worn at the ends, never in what crosses. *(derived: from law 7.15. one walk reads forward from one end and everted from the other, and it is one walk.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| going back is rewinding: the same moves undone in reverse order. | a tape played backward, which is a second drawing and not a walk. on the ring, back is forward with the sign flipped: three quarter-turns undo one. |
| a message has a direction, from and to, written in it. | the envelope, which is written by one end. |

**receipts**

a chip: for decades two assembly notations for x86 have disagreed on which
operand is written first. intel's writes the destination first, at&t's the
source. the instruction is the same instruction. the notation shows which
end the writer stood at *(the field's)*.

mathematics: kauffman factors the square root of minus one into a sign
that alternates from beat to beat and a shift in time by one beat, each
its own undo, whose product squares to minus one *(the field's)*. on the
nine the same two acts are the negated arrival and the swap.

**run it again**

the four mirrors. write the nine cells as pairs (c, a) with c and a in
-1, 0, +1. apply each of the four maps: (a, c); (c, -a); (-c, a);
(-a, -c). count the cells each leaves in place: three each, the centre
(0, 0) every time. the map (-c, -a) leaves one, the centre.

two mirrors. compose every ordered pair of two different mirrors of the
four: 12 pairs. expect no mirror among the results: 4 half-turns and 8
quarter-turns.

the quarter-turn. negate the arrival and then swap: (c, a) goes to
(-a, c). do it twice and every cell is negated. swap first and then
negate the arrival: (c, a) goes to (a, -c), which is a different map for
eight of the nine cells, and each of the two undoes the other.

the other Self. for each of the 81 walks of four stands on the ring, take
its arrivals: each stand minus the next, counted round. reverse the
stands and take the arrivals again. expect, 81 times of 81, the first
arrivals in reverse order with each one negated.

the 48 laps. take the nine cells as pairs of digits. two cells are
neighbours when exactly one of their two digits differs. list every closed
lap that visits all nine cells once, counting a lap and the same lap
walked the other way as one, and ignoring where it starts: expect 48.
write each lap as its word: at each move, which slot changed and by how
much, counted round. reverse the word and negate each amount. expect that
in 0 of the 48 this is the lap's own word, from any starting place.
