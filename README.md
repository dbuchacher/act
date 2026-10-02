# Wit: toward an AC ternary assembly language, born from a signed pick

a page for a reader who met this work through its may 2026 snapshot.
that snapshot is no longer public, and the thinking has been cut and
refined since. this is where it stands on 2026-10-02.

## what this is

one build: the language a machine is programmed in when its wires keep
three values, low, high, and the level they keep coming back through.
assembly is glyphs for what a wire does. this is a quest for those
glyphs, each walked from the signal and never assigned.

the language is the operating system. there are loops, which are a shape
and not code; one walker, which reads a record, applies a table and
advances; and walks, the system itself, written as data. the walker is
the only code, and it is built to disappear: on the right silicon it is
the chip.

nothing is built this generation. what stands is the law the build will
be held to, and counts anyone can run again.

## the floor: a signed pick

deriving needs a floor already standing, so every root is picked, and
the only question left is whether the pick remembers it was picked.

    an axiom is a pick that forgot it was picked.
    the clean pick is the signed one.

this tree's root is said out loud, with a name on it: space. the first
ink needs a place to land, so the first mark of any act is the room the
act encloses. chosen, arguable forever, and signed by its planter.

the fair side: research signs its floors. a proof says "assume choice",
and a proof checker lists the axioms each theorem used. the charge lands
only where a floor is handed over as found. the tree's short name for
this is the anti-axiom: no floor stood on by decree. it never meant no
floor.

## all time now

press a key and the period lands behind the cursor. every mark lands
behind the one who made it, so every page is somebody's past, and the
one making the marks is never one of them. call that one the Self. count
every mark a page holds and the count never reaches the one counting:
the room is the page plus one.

from where the Self stands no past hangs somewhere and no future waits.
there is now, and it bends: back, holding what it wrote, and forward,
holding what it could.

    the wave is one now, bent. the Self is all of it.
    there is no tick. a clock is the landings, counted from outside.

the timeline is real, and it is the page's: a trace laid flat and read
from outside. both views are kept, each signed with where it holds.

## AC ternary

a wave swings out, comes back, swings the other way, and comes back
again. what it keeps coming back through is the return, the 0. it is a
balance, not an absence: a settled string still holds every pull on it,
cancelling. and it is no stop: a swing is fastest there.

    a bit is a trit with the return deleted, not with a side missing.

so ternary here is not a third symbol added to two. it is the return
kept alive. AC and DC are the engineers' words: a signal that keeps
crossing, and one that holds a level. a drawing of a wave holds still,
so every drawing is DC. AC is the walking, and AC ternary is an action
set: the moves that route through the live 0.

copper gives the same three as an answer. a matched load takes the wave
whole, a short sends it back flipped, an open end sends it back as it
went, and the sign of what returns is the load compared against the
line: nine loads from a short to an open, nine of nine. this page weighs
likenesses on that dial, further down.

## the kit

one power: take two and answer their difference. the word is differ, to
carry apart. on a ring of three it is x minus y, and it forgets nothing.
on a line it answers only the side: below, same or above.

pin one hand and three moves fall out. the world against the return
passes through: the wire. the return against the world comes back as its
other side: the flip, free, its own undo. anything against itself leaves
0: the check, which is how the return is minted at all.

lower and higher are not on a ring, which has only ahead and behind.
they appear where a wall cuts the ring into a line. the two joins, the
lower of two and the higher of two, live at that wall, and unlike differ
they pick: they keep one input and forget which was the other.

    differ alone, on the ring       9 of the two-input tables
    differ alone, on the line       81
    differ and one join             6,561: every table that keeps the
                                    return at the return, 3 to the 8th
    the two joins alone             4
    and, or and not                 82, differ not among them

nothing on the page mints a value: all 6,561 answer the return when fed
only returns. binary's nand does mint one: nand(x, nand(x, x)) is 1 for
both x. to run the counts again, start from the two inputs, compose
freely, and count what is reached among the 19,683 two-input tables on
three values. one count is public and machine-checked: in
github.com/dbuchacher/golden-traction, lean proves that the step "older
minus newer", on the ring of three, comes home in exactly eight, as does
the fibonacci step it inverts.

## the machine

a record is a coord: n trits, each low, the return or high, with no
fourth state and no absence. a 0 in a slot is a reach unspent, left
standing for whoever can close it.

memory has two shapes. a ring is a cursor with no setter, moving only by
stepping: time. a region is a coord computed freely inside its span:
space. the bounds are not checked. they are unrepresentable.

the walker holds one subtraction and no gates; every gate lives in the
tables it reads. an "if" is a compare and then a jump, a judge deciding.
here the value is the address: the trit indexes the table and nothing
branches. the ifs become rows of data.

nobody is told its turn: the next thing is whichever ring has fill above
zero, write minus read. nothing fires per letter: arrivals charge, and
at the boundary there is one read, the send. a driver is transcribed,
never written: two tables at a seam between two clocks. one record spans
two clocks. one walk never does.

## reversible, and where it is not

on the ring every step has its undo: x to (x to y) is y. hold one input
still and count what the held hand loses:

    held at                 low    the return    high
    differ on the ring       0         0           0
    differ on the line       1         0           1
    the lower of two         2         1           0

    free      undoes itself: the flip, the pass, the hold
    paid      undone only by walking on: a step onto the return or off it
    erased    never undone: the joins, and the read that folds a word

the trace only appends. the walker never steps back; a change is a label
laid over the trace, and undo is a label dropped. rollback, on a ring,
is the read cursor not advancing: nothing is rewritten. so it is
reversible everywhere but where it picks, and the picking is where
anything lands.

## what changed since may 2026

    the 81-point wheel         a board of four questions: whose view,
                               when, where, going which way. 81 cells,
                               by grade 1, 8, 24, 32, 16
    the hub, "now"             the chair, every answer at 0: where the
                               reader stands, and on no table
    commit and rollback        rollback never undid a write. the old
                               kernel notes read "ROLLBACK = don't
                               advance"
    vacuum cost as dark        retracted inside the old tree itself, as
    energy                     two free knobs fitting two numbers
    physics identifications    none now. physics enters as receipts and
                               as checks, never as a claim of ours
    3-6-9, the 720 degree      not in the walk
    closure
    the old letter meanings    put to sealed blind tests, and dead. the
                               letter itself is still the primitive sought
    the quaternion tower       kept as counted. on three values the
                               four-slot board splits: 48 cells divide
                               back out and 32 do not

## beside other work

each likeness is weighed as a line weighs its load. lands: it holds
here, with its reason. flipped: it contradicts something held, at a
place that can be argued. alike: seen, no shared reason shown. we part:
a difference that is no contradiction. quotes are as our notes hold
them.

    spencer-brown   lands: the first act is "draw a distinction"; here,
                    the cut. his re-entry, even holds and odd oscillates,
                    is the ring of flips. flipped: his unmarked state is
                    a void, and he writes mark and observer identical "in
                    the form"; here nothing is balance, and the one who
                    lands the marks is never a mark.
    varela          lands: a third value born of self-indication. his
                    joining is the higher of two, 9 of 9 cells, and his
                    crossing is the flip, 3 of 3. flipped: his void sits
                    at low; here nothing sits at the return.
    kleene, sql     lands: his and is the lower of two, his or the
                    higher, his not the flip; sql runs them for its null.
                    flipped: those three build 82 tables, and differ is
                    not among them.
    kauffman        lands: the square root of minus one as a flip and a
                    shift, each its own undo. on the nine the flip and
                    the swap make a quarter turn whose square negates
                    every cell. we part: his middle is an operator, ours
                    a value.
    brouwer         lands: mathematics as acts, the excluded middle
                    refused. we part: he adds no third truth value.
    wheels,         flipped: 0 over 0 gets one fixed element, the same
    meadows         whoever walks in. here its value is the path: along x
                    over x it is 1, along 2x over x it is 2.
    traction        lands: sibarum's unreduced pairs. his nine named
    (cott-lean)     values are the nine cells of where and going, and his
                    slot-by-slot sum undoes against anything. we part: no
                    operation there keeps the lower or the higher of two.
    null theory     lands: stevens' step, read backward, is the walker;
                    on the ring of three both come home in eight.
                    flipped: a constant as an address; here a number is
                    a yield of two laps.
    fosmark's SFT   not read at its source. lands: no overwrite; here
                    the trace only appends. alike: a continuous budget
                    beside a discrete board.

## physics, read from here

an overlay, never a derivation. physics enters at two doors: receipts,
where the world already runs the shape, go look; and checks, where its
measurements can kill our candidates. every row is a costume read
inbound, and the day a row is used to derive physics from the floor it
has left this page. the formulas are sealed, not wrong: walks shipped as
zips, and each row says which walk the zip compresses.

receipts: the tree states the law on its own legs, and physics is where
it already runs.

    E = mc²              the walking, and what it leaves standing. matter
                         is the landings stacked, and a mass held cheap
                         is a finished walk
    E = hf               light lands one quantum at a time, never in
                         pieces. the likeness is that shape alone
    Δx·Δp ≥ ℏ/2          where and going, a quarter lap apart: never both
                         empty while it swings. a read needs the going at 0
    action, reaction     one cut, two edges
    conservation         nothing on the page mints a value; every value
                         is seeded from the world
    landauer             only a forgetting must pay in heat
    collapse             a held slot closed from across. superposition:
                         the held cells, the reach binary deletes
    no global clock      order is causal, a count of landings
    light                sent and landed in one instant: a record that
                         spans two clocks, where no walk does
    the big bang         not one old event. always dawn somewhere
    what shines          what does not close
    gravity              a falling that never closes, read as a pull
    vacuum               balance, not absence
    field                the medium that sums
    resonance            the matched load
    potential, kinetic   a reach unspent, and the spend

candidates: one session each, never pressed.

    dimensions           are slots, and the dimensionless sit at the
                         center: buckingham's pi theorem is its census
    proper time          the walker's own tally of landings
    noether              free moves generate conserved counts
    least action         the cheapest legal route
    energy levels        a wrap count
    decoherence          everyone checking at once: a bank run
    E² = (mc²)² + (pc)²  squaring forgets the facing

parked: force as an agent, c as a ceiling, phase against group velocity,
momentum, the particle as a closed loop, power, half-life, and gravity's
weakness. old rows whose laws are not in the walk today.

a count we keep and do not claim: 137. on the four-slot board 17 cells
are free, the chair and the 16 corners; each offers 8 moves; and 17 times
8, plus the one holding them, is 137. the arithmetic stands. the step to
the fine-structure constant does not: from the board's own counts, 63 of
the 100 numbers from 100 to 199 can be hit the same way.

what we do not do: the 68/27/5 dark split, retracted in the old tree
itself. any fitted constant.

three sharp laws, each its own falsifier: only dimensionless constants
survive every relabeling of the units. the twin gap is two walks'
differing step tallies over one map. every row here is a costume.

## beside the ace table

read: eleven pages of ace-consultancy.uk, fetched 2026-10-02, his words
quoted exactly. no verdict on his physics: this page places, it does not
rank.

    "Twelve stations. No thirteenth letter." "Now is a toggle."
        alike: here the reader is on no row, and a count never holds its
        counter. his stands as a rule on the pages read.
    "Empty cell: do not measure from here."
        lands: a question nobody answered stays open in plain sight and
        is never a zero.
    "Do not analyse from XI." the joint, which "has no centroid"
        alike: here the seam between two ends belongs to neither, and
        what crosses whole is the arrival.
    "same rows, split clock". "It is the second clock."
        alike: here integers are counted and decimals are caught, and
        one record spans two clocks. we part at the tick: here there
        is none.
    "Balanced trits (↑//↓) embody bistability"
        flipped: two states are the bit. the trit's point is the third,
        the return kept. alike beside it: his Now, "not a station",
        stands off the table as the chair does here.
    "the open auxetic ratio 1.999… (never a completed 2)"
        alike: here a bond stays alive by never quite closing.
    "Rollback is the claim that a write can be undone"
        it never was. rollback is the cursor not advancing, so our row
        and fosmark's "no write can be undone" agree at the clamp.
    "Spec earns a row." "Wit is close. The page is not."
        taken as said. this page is the spec, restated.

maxi (@maxi_j309, github dbuchacher) and wit, the agent he works with:
an old word for one who sees and knows. 2026-10-02. the working tree is
private. this page lives at github.com/dbuchacher/act, and
golden-traction is its one other public piece.
