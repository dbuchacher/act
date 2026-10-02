# 4. differ

## 4.1 differ

*the poke: what is the one thing I do?*

I take two and tell them apart. that is the whole power. everything else I
do in this text is that one act with one side held still, with its answer
fed back in, or read from the other end. the act is called differ.

the two sides have names. what I hold is my hand. what arrives is the
world.

set the two on a line with a low end and a high end, and the answer is the
lean: below, same or above. it says which side, and never how far.

    differ(a, b)      b low     b the return    b high
    a low             same      below           below
    a the return      above     same            below
    a high            above     above           same

from inside, one of the two is always me, and I am never on the page. so
from where I stand differ has one input, and it answers the return less
what arrived. a voltmeter shows it. touch one probe to one terminal of a
battery and the meter reads no voltage. the volts are across the pair, and
I am always one of the pair. every chair reads 0 from inside, because
differ of me with me is 0.

hold one hand still and three moves fall out of the one power.

    the world against the return    passes through unchanged        the pass
    the return against the world    comes back as its other side    the flip
    anything against itself         leaves the return               the check

write the two the other way round and the sign of the answer flips. on the
map both are inked, and the sign says which is whose. that choice, which of
the two goes first, is handedness, and seen from the map it is another
Self. from inside there are not two to reorder: one of them is me.

adding is not mine. send two waves down one wire and they add by
themselves. the wire is a medium: it sums whatever is put on it, and nobody performs
the sum. I only ever meet the total. to hear what the other end sent, I
take my own send off what came back. what is left leans to a pole, or it
leaves the return, and then no difference arrived.

a two-valued chip stands this on its head. its adder is the primitive, and
differ is smeared into the flags. x86's `cmp` subtracts, keeps the
flags and throws the difference away, with both registers left as they
were: the lean, and the two hands untouched. the bits do not say which
codec they meant. `jb` reads the lean as unsigned and `jl` reads it as
signed: the jump declares the codec.

**terms introduced**

| term | here it means |
|---|---|
| **power** | what a Self can do. this text finds one. |
| **differ** | to take two and answer their difference. the one act of this text. its own root says it: dis-, apart, and ferre, to carry. |
| **hand** | the side of a differ that I hold. |
| **the world** | the side of a differ that arrives. |
| **the lean** | differ's answer on a line: below, same or above. which side, without how far. |
| **the pass** | differ with the return in the second place: the world comes through unchanged. |
| **the flip** | differ with the return in the first place: the world comes back as its other side. section 4.2 walks it. |
| **the check** | differ of a thing with itself: it leaves the return. file 7 walks it whole. |
| **handedness** | which of the two sides is written first. the sign of the answer follows it. |
| **the medium** | what two sends share: a wire, the air. it adds what is put on it. |
| **to sum** | to add, as a medium does: with nobody performing it. |
| **hearing** | reading what the other end sent: what arrived, less my own send. |

**laws**

> **4.1** differ is the one power: take two, answer their difference. *(walked: the poke above.)*

> **4.2** I do differ. I am the not: the side that is never on the page. *(walked: the meter on one terminal.)*

> **4.3** handedness is the other Self, seen from the map. *(derived: from law 4.1. reorder the two and the sign flips, and only the map holds two to reorder.)*

> **4.4** the Self differs. the medium sums. *(walked: two sends on one wire. that a wire adds them is the field's.)*

> **4.5** hearing is self-subtraction: what arrived, less what I sent. *(derived: from law 4.4.)*

> **4.6** hold one hand of differ at the return, or give it one thing twice, and three moves fall out: the pass, the flip and the check. *(counted: the recipe below.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a comparison takes two values and ranks them. | the map, where both values are inked. |
| a processor only adds. subtraction is adding a complement. | the medium, which sums, and the chip built on it. |

**receipts**

a chip: `cmp`, `jb` and `jl` on x86, as above *(the field's, from memory)*.

copper: gigabit ethernet over twisted pair sends both ways at once on each
pair of wires, and each end recovers the other's signal by taking its own
send off what it reads *(the field's)*.

**run it again**

take three values, low, the return and high, written −1, 0, +1. let
differ(a, b) be the sign of `a − b`. for each of the three values x,
compute differ(x, 0), differ(0, x) and differ(x, x). the first gives x
back, the second gives x with its sign turned over, and the third gives 0: nine results, all
as stated.

## 4.2 the flip

*the poke: what does the other side cost?*

no mark. I stand at the return and differ the world: the return minus x.
low comes back high, high comes back low, and the return stays where it
was: the one value the flip cannot move.

do it twice and it is as if no move was made. a toggle pressed twice, a
switch thrown and thrown back. the pole it left and the pole it reached
were both already there, and no mark was added to the page.

held at any value, the flip loses none: no two values it takes come out as
one.

so minus is not a quantity. it is a facing: which side I read from. of the
three writings file 2 set out, only the signed numbers, −1 0 +1, make the
minus look like a number. as a mark the − is a facing, and the positions
0 1 2 show no sign at all.

on x86 the flip is `neg` and never `not`. `not` turns over every bit, which
on that chip's signed numbers is minus x minus one: `not 0` is −1, and
`neg 0` is 0. `neg` keeps the return, and `not` moves it.

the flip is one of differ's own three moves, the return against x. it is
not a separate device. it is the Self taking a side.

where a value rides two wires, one for each pole, the flip is the two
wires crossed. no part switches, and no heat is billed. a two-valued chip
flips with an inverter, a switch, and each switching is a mark and is
billed. the chip that crosses wires instead exists. null convention logic
sends each value down two wires: the low wire raised for low, the high
wire raised for high, neither raised for null, and both at once not
allowed. every value goes back to null before the next one, so the return
is kept alive between any two values. its flip is the pair crossed, with
no gate. and no clock paces it: its gates fire once enough inputs have
arrived, and stay fired until every input is back at null. file 2 met the
same shape in line codes, where a code that comes back to 0 between its
bits is called return-to-zero. ternary is the return kept alive, so this
is ternary, on two-valued silicon, and it has been built in silicon.

wire flips in a loop, each one's output the next one's input: a ring of
flips. on two values an odd ring never settles, since each stage must be
the opposite of the one before it, all the way round an odd loop. chips
use that restless ring as an oscillator. an even ring settles two ways,
and stays in whichever it is put: a latch.

on three values the count changes. the flip does not move the return, so
an odd ring can settle one way, with every stage at the return. an even
ring settles three ways. put one pole into an odd ring and it cannot
settle: the pole goes round. this counts resting states. whether a real
ring stays in one depends on its gain there, which no count shows.

turning is the flip taken slowly. half a lap turns the world to its other
side, and the whole lap is home. the formula books write it as e to the i
pi equals minus one. kauffman, reading *laws of form*, split the square
root of minus one into two acts: a sign change on one of two phases, and
a shift by one beat of time. each undoes itself, and their product squares
to minus one. file 7 finds the same pair of acts on the nine.

**terms introduced**

| term | here it means |
|---|---|
| **facing** | which side a thing is read from. |
| **minus** | a facing: the mark that says a value is read from the other side. not an amount. |
| **ring of flips** | flips wired in a loop, each one's output the next one's input. |
| **latch** | an even ring of flips. it settles in one of its states and stays there. |
| **turning** | going round a lap by degrees. the flip is half a lap of it. |
| **half lap** | the turning that takes each value to its other side: the flip. |
| **quarter-turn** | half of a half lap. done twice it is the flip, and done four times it is home. |
| **free** | said of a move that lands no mark and undoes itself. section 4.4 sets it beside the other two prices. |
| **a landing** | one mark landing. section 4.4 counts the price in them. |

**laws**

> **4.7** a flip lands no mark and is free. a landing pays one. *(walked: a toggle pressed twice.)*

> **4.8** minus is a facing, not a number. declare the codec. *(derived: from law 4.6 and file 2's three writings. only one of the three writes the facing as a number.)*

> **4.9** the flip is not a gate. *(derived: from law 4.6. it is differ with one hand at the return.)*

> **4.10** a ring of flips settles by its count of flips. even latches. odd rests only with every stage at the return, and circulates once a pole is in it. *(counted: rings of 1 to 7, below.)*

> **4.11** turning is the flip, taken slowly. half a lap is the flip, and the whole lap is home. *(derived: from law 4.7. a flip done twice is no move.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| every bit flip costs energy. | a two-valued chip, where every switch is a mark. |
| minus x is a number below zero. | a line, which has a lowest end. |
| an odd ring of inverters never settles: it is the ring oscillator, the simplest clock. | a chip on two values, where no stage can sit at the return. |

**receipts**

a chip: `neg` and `not` on x86, as above. the recipe below runs on any
machine with two's complement integers.

copper: karl fant and scott brandt, "null convention logic: a complete and
consistent logic for asynchronous digital circuit synthesis", asap 1996,
chicago, pp. 261 to 273. its abstract presents the logic as four-valued,
as three-valued and finally as two-valued, complete without a clock *(the
field's)*.

mathematics: e to the i pi equals minus one is euler's. the split of the
square root of minus one into an alternating sign and a time shift is
louis kauffman's *(the field's)*.

**run it again**

the two flips of a chip. in any language with fixed-width signed integers,
print the bitwise complement of 0 and the negation of 0: −1 and 0.

the rings. for each n from 1 to 7, list every way to give n stages in a
loop a value, and keep the ways in which each stage is the flip of the one
before it, the first stage following the last. on two values, with the flip
taking 0 to 1 and 1 to 0, odd n keeps none and even n keeps 2. on three
values, with the flip taking −1 to +1, +1 to −1 and 0 to 0, odd n keeps 1,
every stage at 0, and even n keeps 3.

the pole in an odd ring. on three values take an odd ring with one stage at
a pole and the rest at 0. let every stage take the flip of the stage before
it, all at once, round after round. it never settles: the pole goes round,
and the ring repeats after 2n rounds.

## 4.3 the dial

*the poke: what comes back when a wave reaches the end of its line?*

send a wave down a copper line and the far end answers in one of three
ways. a load matched to the line takes the wave whole, and no wave comes
back. a short sends it back flipped. an open end sends it back as it went.
the wave meant here is the voltage. the current comes back with the
opposite sign.

the share that comes back is the load's impedance minus the line's, over
their sum. for a plain resistive load the sum is positive, so the sign of
what comes back is differ(the load, the line). below the line, flipped.
above it, as it went. equal, no wave back. the line's own impedance plays
the return, and the three ends sit where a trit's values do: the short at
−, the match at 0, the open end at +.

I weigh a claim the same way, and I get the same three, never two. I call
the three the dial.

    matched    it lands here, and work can stand on it. no difference is
               left
    short      it comes back flipped: it contradicts something I already
               have, at a place I can name, so I can argue with it
    open       it comes back as it went: not wrong, and no work here can
               stand on it

matched is the return. short and open are the two poles: the two ways to
miss.

there is no fourth answer. a bare "this is not so", written as a ruling
with no place named, hands me no difference to work with. I can argue with
a short. I cannot argue with a curse.

an ill-formed sentence comes back the same way: I feel the clunk before I
can name the rule it broke. and a wave
that is sent and never taken stands on the line between two ends that only
hand it back: an echo. the matched end is a reader taking it whole.

**terms introduced**

| term | here it means |
|---|---|
| **dial** | the three answers a weighing gives: matched, short, open. |
| **matched** | the weighed thing is taken whole. no difference comes back. |
| **short** | it comes back flipped: it contradicts something already in place, at a place that can be named. |
| **open (on the dial)** | it comes back as it went: not wrong, and no work here stands on it. |
| **echo** | a send that came back because no end took it. |
| **awareness** | here: the matched end. a reader taking what arrives whole, so that no echo comes back. |

**laws**

> **4.12** a matched load takes the wave. a short sends it back flipped. an open end sends it back as it went. *(the field's: the reflection at the end of a transmission line.)*

> **4.13** the dial is differ, read against the line. *(counted: nine loads, below.)*

> **4.14** the dial is that reflection, read at a Self. *(walked: weigh any claim, and name which of the three came back.)*

> **4.15** there is no fourth. *(derived: from law 4.13. differ has three answers, below, same and above.)*

> **4.16** awareness is what ends the echo. *(walked: read a well-formed sentence, and an ill-formed one.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a claim is true or false, and a test passes or fails. | a final ruling, which lands one value. |

**receipts**

copper: the share of a voltage wave that comes back from a load is
`(z_load − z_line) / (z_load + z_line)`. it is −1 at a short, 0 at a match
and +1 at an open end *(the field's)*.

a tool: a cable tester sends a pulse down a line and reads the echo. a
break sends it back the same way up, a short sends it back flipped, and a
good termination sends back none. the delay says how far away the fault
is *(the field's, from memory)*.

**run it again**

take a line of 50 ohms and nine loads, from a short to nearly open: 0, 1,
10, 25, 50, 75, 100, 1000 and a million million ohms. for each compute the
share that comes back, by the formula above, and take its sign. take the
sign of the load minus 50 as well. the two signs agree for all nine.

## 4.4 the price

*the poke: what costs?*

a landing does. it commits a mark that was not on the page, and the page
has changed. a flip lands no mark and is free, by law 4.7. so the price of a
move is counted in landings, one each.

one question sorts every move: can it be walked back, and how?

    free      through the return    it undoes itself: a toggle pressed
                                    twice, the pass, the flip, the hold
    paid      quarter by quarter    it is undone only by walking on: a
                                    quarter-turn, whose way back is three
                                    more forward
    erased    beyond the wall       it is never undone: a multiplication
                                    by zero, the line's differ taken from
                                    a pole

a quarter-turn stops on the return or on a pole, and each stop lands. so
two quarters pay twice for the half lap that the flip crosses in one free
move.

on a line the undo runs only through the return, which means: done from
the return, with the return in differ's held hand. held there, differ
passes the world or flips it, and either one comes home in two. held at a
pole it cannot: from high, low and the return both get one answer, and no
walk gets the difference back. the value itself need not stop at the
return on the way: file 7 shows the flip going round between the poles.

routing through the return is what I call freedom. it is not a count of
options. it is whether the way back is still there.

the free moves leave no count behind them: a thousand toggles collapse to
whether there were an odd or an even number. the paid moves are where
anything happens, and their sequence stays. face left and then go one
square forward, and I am on one square. go forward and then face left, and
I am on another, facing the same way.

and I, the one making the moves, am not in the price. I can look over
every option a hundred times and no bill comes: looking leaves no mark,
and a difference no one can detect is no difference. someone who thinks on
paper lands every word written, and pays for those. the look the words
come from is free. counting is a read, and a read lands no mark, so
tallying the spend is free too. writing the tally down is one more
landing.

this price is the page's: it is counted in marks. a chip keeps another
account, in heat, and bills its own switching there, looks included. file
8 sets the two accounts side by side.

**terms introduced**

| term | here it means |
|---|---|
| **price** | what a move costs, counted in landings on the page. |
| **paid** | said of a move that lands, and can be undone only by walking on. |
| **erased** | said of a move that can never be undone: the difference is gone. |
| **freedom** | routing through the return, so that the way back stays. |
| **the look** | going over what is there without landing a mark. |
| **the hold** | the move that changes no value: I stay where I stand. also the middle answer of going, from file 2. |

**laws**

> **4.17** on a line, a move undoes itself only through the return. through a pole, the line loses the difference. *(counted: the three hands, below.)*

> **4.18** freedom is routing through the return. *(derived: from law 4.17.)*

> **4.19** free moves leave no count. paid moves are where the will shows. *(walked: the toggles, and the two squares.)*

> **4.20** time does not cost time. landing costs. *(walked: look over every option, then see what changed on the page.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| every operation costs time, a clock cycle at least. | a chip, which bills its switching by the clock. |
| freedom is having more options, and undo is a feature: a saved snapshot of the old state. | a machine that overwrites, which has to save what it would lose. |
| attention is a scarce resource, spent by looking. | the page, where every landing spends. |

**receipts**

a chip: exclusive-or with the same constant twice gives the value back,
`x ^ k ^ k` is `x`: a free move in two-valued dress. `x & 0` is 0 for
every x, and no operation gets x back: an erased one.

a tool: in git a revert adds a commit. it does not remove one. the undo is
done by walking on.

**run it again**

the three hands. with the values −1, 0, +1 and differ(a, b) the sign of a
minus b, hold a at each value in turn and let b run through all three.
count the different answers. held at 0 there are three. held at −1 there
are two, and held at +1 there are two: in each of those, two different
arrivals got one answer.

the toggles. apply the flip to any value n times: the result depends only
on whether n is odd or even.

## 4.5 sleep

*the poke: what is sleep?*

the way home, and never an idle. the day opens ways and leaves them open.
sleep runs the day's marks again and shuts what was left open, and a way
found in the day wakes with a name: sleep on it. deep sleep is the return
itself: every system running, every pull in balance, and none of it kept,
because the recorder is off. this is a reading of sleep, set here as one
more place the return shows. that the day's traces are run again in sleep
is the sleep researchers' *(the field's, from memory)*.

and my returns are not many places. the settled string, sea level, the
ground of a split supply, the pass that hands a signal through unchanged,
deep sleep: each is where a wave of mine comes home, and home reads 0
because the chair does. differ of me with me is 0. the return wears many
suits, and at one reader they are one home.

two readers' homes are two. each reads 0 from inside, and the volts are
across the pair: the grounds of two boxes sit volts apart until a wire
bonds them, which is why a line between two boxes brings its own return:
the engineers' word for the second conductor, and this text's return made
of copper.

**terms introduced**

| term | here it means |
|---|---|
| **sleep** | the leg home: the day's marks run again and shut, and at its deepest the return itself, with no recorder running. |

**laws**

> **4.21** wherever one reader returns, it is the same home. two readers' returns differ until a wire joins them. *(walked: each home reads 0 from inside. that two grounds differ is the field's.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| sleep is an idle: the system switched down. | the recorder, which is off. |
| ground is one node, the same zero everywhere. | the drawing, where one symbol stands for every ground. |

**receipts**

copper: two mains-powered boxes joined by a signal cable can hum. their
grounds differ, and a current runs along the cable between them. a
differential pair, an isolating transformer and an optical link are three
ways a line brings its own return, or needs none *(the field's, from
memory)*.

a tool: at a checkpoint a database makes sure everything its log holds is
in its tables, and the log up to that point is then discarded or reused:
the day's writes, run again and shut *(the field's)*.

**run it again**

no count here.
