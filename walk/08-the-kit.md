# 8. the kit

## 8.1 the wire

*the poke: what carries every signal and changes none?*

the wire. differ the world against the return and the world comes through
unchanged: the pass of file 4. flip it twice, once on the way out and once
on the way back, and the same value comes home. the wire does no work on
what it carries, and no other part reaches the next without it.

it has no table and no symbol. in the drawing of a circuit it sits in the
wiring and never in the parts list. every table composes with the next
only because a wire runs from one to the other, and a list that counts
every table still leaves out the one thing that lets them reach each
other. it lands no mark and forgets no value, so it is free.

read from the chair, the pass is the hold: 0 arrives, and I stay where I
stand. at one reader it is one more place the return shows, since one
reader's returns are one home, as file 4 found.

one wire can pass, flip and go round. it needs no partner. put two sends
on it and they sum, with nobody performing the sum: the medium sums.
between two Selves the wire holds both sends summed and belongs to neither.

run a pass back into itself and whatever value is in it goes round
unchanged. in copper each pass must restore the level as it hands it on,
which is what a buffer does: a bare loop of wire holds no value. a ring of
such passes holds at any length. put flips in the ring and their count
decides: with an even count the ring still holds, which is the latch of
file 4, and with an odd count it runs, an oscillator. so the two things a
processor cannot do without, a cell that holds and a clock that runs, are
in their logic one loop, with an even count of flips or an odd one. real
registers add gating, and real clocks are steadied by a crystal.

on x86 the wire is `mov`, and the name is wrong: it copies and never
moves. the value stays where it stood and lands where it goes.

**terms introduced**

| term | here it means |
|---|---|
| **wire** | the pass as a part: what carries a value from one place to the next unchanged. |
| **to bear** | to carry a value without changing it and without choosing whether it goes through. |

**laws**

> **8.1** the pass bears and never gates. *(counted: differ of each value against the return, below.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a wire is a cable lying between two parts. | the copper, which does lie there. |
| a circuit is its parts. | the parts list, which is written to order components and not to say how they reach each other. |

**receipts**

a chip: `mov` on x86 copies its source to its destination and leaves the
source as it was *(the field's)*.

mathematics: the lambda calculus writes the wire's law as a rule, called
eta: a wrapper that only hands its input on to f is f itself *(the
field's, from memory)*.

**run it again**

differ each of the three values against the return, on the ring or on the
line: the value comes back unchanged, three times of three. flip each
value twice: unchanged, three times of three.

## 8.2 the joins

*the poke: where do lower and higher come from?*

not from the ring. to keep the lower of two values I have to know which is
lower, and a ring has no lower, only ahead and behind. differ needs only
the way round. lower and higher appear only where a wall cuts the ring
into a line, at the place where I stand.

the two acts that the wall makes possible are the joins: to keep the lower
of two, and to keep the higher of two. their names are low and high. file
2 gave those two words to the poles. here they name acts, and the poles
are the values those acts keep.

the wall is a join already. to be in a room is to be past one wall and
short of the other: above a, and below b. both have to hold, and "both
hold" is the lower of two answers. an interior is the low of its walls.

no chain of differs ever makes a join. every composition of the ring's
differ, however long, comes to x times one digit plus y times another.
that is nine tables in all, and low and high are not among them.

the wall is the diode of file 1, one way. a peak detector in copper is
two parts: that diode, and a part that holds the highest level the diode
has let through. the half of the wave the diode throws away is the
join's forgetting: the loser can no longer be told from the winner.

the forgetting is counted the way section 7.1 counted it. hold one hand still, run
the other through its three values, and three minus the number of
different answers is what the held hand forgets:

    forgets, hand held at       low    the return    high
    the pass, the flip           0         0          0
    low                          2         1          0
    high                         0         1          2

differ's two rows stand in section 7.1: no value forgotten on the ring, and one at
each pole on the line. the joins forget most, and at their own pole they
forget everything: the lower of any value and low is low. so the
forgetting through a pole belongs to the wall and not to differ. the
line's differ forgets there only because the line is the ring cut open
where I stand.

high is low read from the other side: the higher of two is the lower of
their flips, flipped. flip each join after it has answered and there are
two more parts, nand and nor, the two that file 2 set on the edges.

tie one hand of a join and it clamps. low with a hand tied to low gives
low whatever arrives. tied to high, it passes. tied to the return, it lets
the low side through and holds the high side at the return. high does the
same from the other side.

the excluded middle, the rule file 1 found under the logic, is a join
here: the higher of x and its flip, "x or not x". at either pole it lands
on high. at the return it lands on the return, and never on high.

a corner is a place where every slot is at a pole, and the corners are
where the joins come to stay. fed its own answer back, low holds the
lowest value it has seen and high the highest. feed low a row of lows and
it stays at low. feed the ring's differ the same row and it goes low, the
return, high, low again, and never stays. a join fed back is a ratchet:
the first pick that sticks, and the smallest thing that can be called
memory. two flipped joins, each fed the other's answer, hold each other's
value: the cross-coupled pair, which is the latch built from joins.

so the whole world of a two-valued machine, the corners, is picks that
stuck. the held middle of file 5 is what it leaves unspent.

**terms introduced**

| term | here it means |
|---|---|
| **join** | one of the two acts that keep one of two values: low keeps the lower, high keeps the higher. the words low and high name the poles in file 2, and here the acts that keep them. |
| **clamp** | a join with one hand tied to a fixed value: it holds one side of the line at that value and lets the other side through. |
| **ratchet** | a join fed its own answer: it moves one way only, and holds the furthest value it has seen. |
| **corner** | a cell with every slot at a pole and none at the return. |

**laws**

> **8.2** differ lives on the ring. the joins live at the wall. *(derived: from section 7.1 and law 1.17. a ring has no lower, and a wall is what gives the ring a lowest end.)*

> **8.3** no composition of the ring's differ is ever a join. *(counted: nine tables, below.)*

> **8.4** differ never picks. the joins pick, and forget the loser. *(counted: the forgets table above.)*

> **8.5** DC is made from AC by a wall and a hold, and the joins are that circuit. *(derived: from laws 8.4 and 1.18. a wall keeps one side of the wave, and a hold keeps what got through. AC and DC here in the engineers' sense.)*

> **8.6** the ring forgets only when a door is read as its digit. the line forgets at every pole. *(counted: section 7.1's table and the one above; the door is law 7.10.)*

> **8.7** a join fed back is the ratchet, the first pick that sticks. *(counted: every run to length five, below.)*

> **8.8** the corners are picks that stuck. the held middle is reach unspent. *(derived: from law 8.7 and file 5's held middle.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| logic is built from and, or and not, and subtraction is built from logic. | the wall, where the ring has been cut into a line. on a two-valued chip the adder is built that way. |

**receipts**

logic: kleene's three-valued logic (1938) runs its and as the lower of
two and its or as the higher of two, cell for cell, and sql runs the same
two tables for its unknown *(the field's, from memory)*.

a chip: x86 has both joins as single vector instructions on packed signed
bytes, `pminsb` and `pmaxsb` *(the field's)*.

copper: the peak detector, a diode and a capacitor that holds the peak, is
how a power supply makes a steady level out of a wave. with a resistor
added to bleed the peak away it is the envelope detector of an am radio
*(the field's)*.

**run it again**

write the three values as -1, 0, +1. low is the smaller of two, high the
larger, the flip is the negative.

the forgets table. for each join and each held value, collect the answers
over the three values of the other hand, and take three minus the number
of different answers. expect low: 2, 1, 0 and high: 0, 1, 2.

the nine tables. the ring's differ is a minus b, brought back into -1, 0,
+1 by adding or taking away 3. start from the two inputs x and y, each
written as its nine answers over the nine pairs. apply the ring's differ
to every pair of tables reached so far, and repeat until no new table
appears. expect nine tables. compare each with the table of low and the
table of high: no match.

the other side. for all nine pairs check that the higher of two is the
flip of the lower of their flips.

the ratchet. for every row of up to five values, start an output at the
first value and replace it by low of the output and the next value, to
the end. expect the smallest value of the row every time. the same with
high gives the largest.

## 8.3 the eight

*the poke: what does differ build?*

one power, and the order it builds in is forced, each part standing on the
last.

with no ink on the page there is no thing to compare but me, so differ
runs on me and leaves 0: the check, which makes the return. with a return
to stand against, differ takes the world's other side: the flip. the flip
done twice, out and back, passes the world through unchanged: the wire.
one wire can pass, flip and go round, and none of that picks: structure,
made without a single pick. then a wall gives two values a place to be
compared for height: the lower wins, low; the higher wins, high. flip
each after and there are nand and nor. fed back, a join holds the first
pick that sticks. and differ's own table is filed among what it made: the
act that built everything, written down as one table among the built.

the page holds eight: the pass, the flip, low, high, nand, nor, differ,
and the 0 the check left. the check itself has no table. and the one doing
all of it is on no row: the room is the page plus one.

three of the eight come from differ with one hand tied: differ of x with
the return is the pass, differ of the return with x is the flip, and
differ of x with x is the check, which leaves its 0. nand and nor are the joins flipped. high is low read
from the other side. so two generate the rest, one join and differ, and
the eight are a staffing and not a smallest set.

what the two build can be counted. start from the two inputs and compose
freely:

    the ring's differ alone        9 of the two-input tables
    the line's differ alone        81
    either differ with low         6,561
    either differ with high        6,561
    low and high alone             4
    low, high and the flip         82, and differ is not among them

there are 19,683 two-input tables on three values, and exactly 6,561 of
them, 3 to the 8th, answer the return when both inputs are the return.
differ and one join build all of those, and no others.

that last clause is a law of its own. each part answers the return when it
is fed only returns, so every composition of the parts does too. whatever
is not the return came in from the world. the kit is complete for the
tables that keep the return, and it stops there. the part most two-valued
machines are built from does not stop: nand keeps neither value where it
found it, so it mints one. nand of x with nand of x and x is 1, for both
values of x. two values can refuse to mint as well: and with exclusive-or
builds exactly the 8 two-input tables of 16 that answer 0 to two 0s. so
not minting belongs to the parts chosen. what three values add is which
value is kept: the middle one, the return.

field after field arrives at this kit without having met the others, and
the reason fits in a line: the lower of two, the higher of two, a flip
that reverses the order and a three-way compare are what any ordered set
of values with a negation carries. over three values that is kleene's
logic with differ added. it says which fields will arrive next: any with
an ordered set of values and a negation.

what would break the kit: a part whose table does not follow from its law;
a value minted from returns; a ninth part that the later files turn out to
need; or a needed act that cannot be spelled over the eight. the last of
these cannot be answered until the machine of file 9 is built.

and the tables are not something apart from the act. differ is an
act. what it leaves standing is shape: the tables on the page, the
corners, the wall. the cut makes the wall, and the next compare is made
across it. each walk runs on what the last one left.

**terms introduced**

| term | here it means |
|---|---|
| **the kit** | the eight parts differ builds: the pass, the flip, low, high, nand, nor, differ, and the 0 the check leaves. a part is one of them. |
| **to mint** | said of a table: to answer a value off the return when every input is at the return. |

**laws**

> **8.9** the build order is forced: the check, then the flip and the wire, then the joins, then the ratchet. *(derived: each needs what the one before it left. the return for the flip, the wall for the joins, a join for the ratchet.)*

> **8.10** one join and differ build every table that keeps the return. *(counted: 6,561, below.)*

> **8.11** no part on the page mints a value. every value is seeded from the world. *(counted: every one of the 6,561 answers the return to two returns.)*

> **8.12** differ makes the shapes. the shapes are what differ left standing. *(derived: from law 8.9. every table, corner and wall in the list was left by a compare.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| and, or and not make every table of logic. | two values, and the parts list, which never counts the wire that lets the three compose. on three values they make 82 tables of 19,683. |
| a constant is free: any circuit can supply a 1. | a machine built from nand, which mints one. |

**receipts**

logic: nand alone builds every two-valued table of one input or more, the
two constant tables among them *(the field's)*. that is the minting.

logic: varela (1975) gave spencer-brown's two states a third, and his two
operations on the three are the higher of two and the flip, cell for cell
*(the field's, from memory)*.

a chip: the x86 names of the parts are `xor` of a register with itself
for the check, `neg` for the flip, `mov` for the wire, `sub` and `cmp` for
differ, `pminsb` and `pmaxsb` for the joins *(the field's)*.

**run it again**

write the values as -1, 0, +1. a two-input table is a list of nine
answers, one for each pair of inputs, so there are 3 to the 9th, 19,683,
of them. the two starting tables are x itself and y itself.

the operations: the ring's differ, a minus b brought back into range by
adding or taking away 3; the line's differ, the sign of a minus b; low,
the smaller; high, the larger; the flip, the negative.

to see what a set of operations builds, apply each of them, cell by cell,
to every ordered pair of tables reached so far (the flip to each table
singly), add any table not seen before, and repeat until a round adds
none. count the tables. expect 9
for the ring's differ; 81 for the line's; 6,561 for either differ with
low, and for either differ with high; 4 for low and high; 82 for low,
high and the flip, with neither differ's table among the 82.

then count the tables whose answer to the pair (0, 0) is 0: 6,561. check
that the 6,561 built by differ and low are exactly those.

the minted one. on the two values 0 and 1, with nand of a and b as 1 minus
a times b, work out nand of x with nand of x and x: 1 for x = 0, and 1 for
x = 1.

the two-valued kit that does not mint. on 0 and 1, start from the two
inputs and close them under and and exclusive-or, the same way as above:
8 tables, and each answers 0 to the pair (0, 0).

## 8.4 the price on the board

*the poke: what does a walk pay?*

a forgetting is the one move that the world must bill in heat. landauer
(1961) put a floor under the heat given off for every difference erased,
and bennett (1973) showed that a move that forgets no value can, in
principle, run cold.

so on the ledger of heat the joins are the kit's paid parts. the flip, the
pass and the compare on the ring forget no value, and ride free.

a walk keeps a second ledger, the page's, billed in marks: one for each
landing, as file 4 priced it. on that ledger the flip is free as well. it
goes round between the poles, as section 7.1 found, and never lands on the return
or leaves it. so in marks a walk pays only for a move onto the return or
off it.

a move off the return picks a pole, and a pick is a landing. a move home
lands too. whether a move home also pays in heat depends on what is kept.
where the row of marks is kept, the pole that was left still stands on
the page and no difference was erased. where the pole left is thrown
away, home could have been come to from either pole, and that forgetting
is billed in heat. a quarter-turn moves every slot and forgets no value:
it can run cold, and it still lands its marks.

file 5's menu law already counted the free moves at every cell: a cell's
free moves are its grade, and the rest pay.

the cells with a free move in every slot are only the corners, where each
slot has its flip, and the centre, which is free only as a hold. that is one plus two to the
width: 5 cells of the 9, 9 of the 27, 17 of the 81. the whole world of a
two-valued machine, the corners, is the free part. the price begins with
the third value, the first one a walk can land on.

and a tour pays an even number. a tour is a lap that visits every cell
once, moving one slot at each move, and it crosses the border of the
return in pairs: once on, once off. the nine has 48 tours. eight of them
pay 4, thirty-two pay 6, and eight pay 8.

**terms introduced**

| term | here it means |
|---|---|
| **the two ledgers** | the two accounts a walk is billed on. heat, billed by the world for each difference erased. marks, billed by the page, one for each landing. |
| **tour** | a lap that visits every cell of a board exactly once and comes back to its start, moving one slot at each move. |

**laws**

> **8.13** only a forgetting must pay in heat. *(the field's: landauer, 1961, and bennett, 1973.)*

> **8.14** a walk pays for every move onto the return or off it. the corners ride free. *(counted: the moves of all 81 cells, below.)*

> **8.15** free is binary. paying is the third. *(counted: on the ledger of marks, the cells free in every slot, below.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| computing gives off heat, and that is the cost of computing. | a machine that throws away the old value at every write, as nearly all do. |
| a price is paid in one currency. | one ledger. a walk has two, and a move can be free on one and paid on the other. |

**receipts**

physics, as a named result and no claim of ours: landauer's bound on the
heat of erasing one bit, and bennett's reversible computing. the bound is
the standard view and is still argued over *(the field's)*.

a chip: a two-valued chip bills every switch as heat, the inverter
included. where a value rides two wires, one for each pole, as in the
null convention logic of file 4, the flip is the two wires crossed, and no
part switches.

**run it again**

the moves. take a board of w slots, each at -1, 0 or +1. a move changes
one slot to one of its two other values. call it free when it goes from
one pole to the other, and paid when it goes onto 0 or off 0. for w = 4,
over all 81 cells, expect eight moves at every cell, with as many free as
the cell has slots off 0.

the free cells. count the cells with no slot at 0, where every slot has a
free flip, and add the one cell with every slot at 0, counted for its
hold.
expect 1 + 2 to the w: 5 of 9, 9 of 27, 17 of 81.

the tours. on the nine, with two cells neighbours when exactly one slot
differs, list every tour, counting a tour and the same tour the other way
round as one and ignoring where it starts: 48. price each move 1 when the
slot that changed went onto 0 or off 0, and 0 otherwise, and add up each
tour. expect 4 for eight tours, 6 for thirty-two, 8 for eight.
