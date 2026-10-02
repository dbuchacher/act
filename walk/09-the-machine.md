# 9. the machine

## 9.1 the layers

*the poke: what is the machine, and why build it now?*

the status first, plainly. none of this machine is built. an earlier build
ran pieces of it, and where a figure from that build is quoted below, the
text says so each time. what this file states is the design the build is
held to.

a machine is a power with its mechanism shown. what runs in it is no
substance: telling this level from that is the job of a transistor, and
it is the job of a neuron. intelligence, as file 5 found, is a cut
performed, and the cut does not ask what it runs on.

the operating system is three things.

    loops        circles of slots, gone round by stepping. a shape, and
                 not code
    the walker   the one piece of running code
    walks        the system itself, written as data

done looks like this. a key is pressed and lands as a record in a loop. a
walk consumes it. a pixel responds. between the key and the pixel no code
runs but the walker. then the same bytes, started from a thumb drive, do
the same with no other system under them.

why now. every piece has shipped for decades, in private silos: game
engines, trading systems, network stacks that go round the kernel. it
never spread, because a fixed record is a shared schema, and a crowd of
people cannot keep one. formats like json buy flexibility against that.
an agent holds a whole schema in hand at once, so that limit is gone:
wherever two programs settled on a frozen lowest format because their
authors could agree on no more, the two ends can now simply agree. it is
not free. whoever reads a language of glyphs still pays per glyph. what
is gone is the need for the lowest format.

and the speed is deleted layers, not the language. the crossing into the
kernel, packing and unpacking, parsing, bursts of allocation, bytes
duplicated from buffer to buffer: each goes to zero. timed in electron
apps and in native gtk apps alike, two to eleven milliseconds of a
sixteen millisecond display frame went to work that draws no pixel
*(measured: in an earlier build, on the tree's own record; not re-run for
this text)*.

an emulator pays on its inner routing and saves on every layer it
deletes. the cost is the encoding, and a table all but erases it. on the
first walker's bench (runs E139 and E140), a three-valued gate kept as a
table of nine bytes, sixteen of them per vector instruction, cost 1.52
times the native two-valued operation at the same width, and the same
gate done as arithmetic on the digits cost up to twenty times
*(measured: in an earlier build, on the tree's own record; not re-run for
this text)*. three values do not beat two at arithmetic. the win is the
deleted layers.

the layers are there for someone who is gone. every tool on a unix
command line asks the kernel for structured data and then prints it as
text for human eyes. listing a folder runs fork, exec, readdir, format,
write, pipe, parse, render and read: nine acts where one structured
request would do. maxi built a whole terminal for this machine, thirteen
crates and 933 tests, and then asked who it was for: a human who reads
text. he deleted it. it took building it to see it should not exist.

so the aim is not an operating system that ships. it is the language an
AC ternary machine is programmed in. the OS is written in that language,
all but the walker, and the walker is what the language runs on.

**terms introduced**

| term | here it means |
|---|---|
| **layer** | work between an input and its result that makes none of the result: a crossing into the kernel, a packing, a parse, an allocation. |
| **the OS** | the operating system of this build: loops, one walker, and walks. section 9.2 says where it sits. |
| **loop** | a circle of slots gone round by stepping: the shape memory takes for whatever arrives in order. never a stretch of code that repeats. section 9.3 names it by its shape, a memory ring. |
| **walker** | the one piece of running code. it reads a record, applies a table and advances. section 9.4 walks it. |
| **walk (the machine's)** | a string of records the walker goes through in order. data, never code. it shares its word with this text's walk because it is the same act: going through in order. |
| **record** | the machine's one unit of data, of fixed width. section 9.5 walks it. |
| **table** | a list of results indexed by a value, so that a value is the address of its own result. every gate of this machine is kept as one. |
| **emulator** | the walker written out in a two-valued chip's instructions, standing in for a chip that runs it directly. |
| **host** | another operating system running under this one while it is being built. |

**laws**

> **9.1** the OS is loops, one walker, and walks as data. *(picked: a design, signed by the tree. the usual choice keeps the system as code and passes the data through it.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| an operating system is a large program that manages other programs. | the systems in use today, where the system is code. |
| hand-written assembly is what makes code fast. | the innermost repeated instructions of a program. the larger win is the layers deleted. |

**receipts**

a tool: listing a folder on unix, as above. the kernel crossings among the
nine can be watched with any system-call tracer.

a chip: an nvme drive already talks to its computer through rings of
fixed records and a signal that a position moved. section 9.3 uses it *(the
field's, from memory)*.

**run it again**

no count here. the two timings are measurements of an earlier build.

## 9.2 the seam

*the poke: where does the machine live?*

not in the box. I am a device to the computer, and it is a device to me:
each of us is a loop the other reads and writes, and what sits between us
is two spec sheets face to face. that border is the operating system.

file 7 named the door in the middle of a walk the seam. the machine's
seam is that place at full size: the border between two devices, which
neither one owns.

the picking happens in the between, and picking between is intelligence
(file 5). read from here, a machine that is the seam is not artificial.
it is intelligence, performed at the seam, by whoever is there.

**terms introduced**

| term | here it means |
|---|---|
| **device** | anything with a spec sheet that another reads and writes: a keyboard, a screen, a disk, a chip, a person at the keys. |
| **spec sheet** | what a device takes and what it gives, written down. |
| **the seam between two devices** | where two spec sheets touch. neither device owns it. |

**laws**

> **9.2** the OS is the seam between two devices. *(walked: the poke above. find the place where the keys I press become the machine's, and say which side owns it.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| an operating system lives inside the computer. | its code, which is stored there. |
| a machine that picks is an artificial intelligence. | the mechanism, which is built. the picking is done at the seam. |

**receipts**

a chip: a keyboard controller and a processor share no code. each follows
its own datasheet, and one small shared record crosses between them.

**run it again**

no count here.

## 9.3 the ring and the region

*the poke: what shapes does memory come in?*

two.

    a ring      a cursor with no setter, moving only by stepping.
                what it keeps is in order: time, delivery
    a region    a position computed freely inside a span.
                what it keeps stays put: space, residence

file 7's ring was three places gone round, with no lowest and no highest,
only ahead and the other way. a memory ring is that shape at any size:
slots in a circle, a cursor that goes from one to the next, and after the
last slot the first again. file 3's region was a stretch of the board. a
memory region is a stretch of memory. from here to the end of this file,
ring means the memory ring unless the text says the ring of three, and
region means the memory region.

memory itself is file 8's word made large: each slot is a pick that
stuck, and the machine's memory is slots in these two shapes.

running off the end of a ring cannot be said. there is no end, and the
cursor has no setter. a position of the wrong width for its region is a
different record, and it does not parse. so neither fault needs a test
while the machine runs. a full ring is another matter: fill says so, and
section 9.8 says what a full ring does.

disk and memory are one design. a fast disk already is the primitive: a
ring for requests, a ring for results, and a doorbell to say a cursor
moved. what differs between disk and memory is one number, the delay.

the ring's own pieces, in the words of files 2, 4, 6 and 7:

    the write cursor      high: the reach, where the next record goes
    the read cursor       low: the landed, what has been taken
    fill                  write minus read: differ, and the one thing a
                          reader ever asks of a ring
    advancing the write   the fall: a record leaves its writer
    advancing the read    the rise: a record arrives
    the slots under it    the pass: the wire under all of it
    a cursor come round   the carry: the lap closed, file 7's circle. it
                          is not the check, which is the retrace
    rollback              free: the read cursor does not advance

rollback gets a paragraph of its own, because the word is usually heard
as an undo. on a ring it is the read cursor staying where it is. the
record is still there. no write was reversed, and section 9.4 says why none ever
is.

safety is by absence. a capability never given has no surface to attack,
and a vocabulary that could say "treat this value as a raw address,
anywhere in memory" would defeat every table in this file. on a host, the host catches the fall.
with no host under the machine no one does, so the defense lives in how
things are written, and never in a test made while running.

**terms introduced**

| term | here it means |
|---|---|
| **memory ring** | slots in a circle, with cursors that only advance. what arrives in order is kept here. section 9.1's loop, named by its shape. |
| **memory region** | a span of slots, addressed by a position computed inside the span. what stays is kept here. |
| **cursor** | a position on a ring that can be advanced and cannot be set. |
| **fill** | the write cursor minus the read cursor: how many records wait. |
| **bound** | the limit of a ring or of a region. here it is a fact of how positions are written, never a test. |
| **rollback** | the read cursor not advancing. no write is undone. |
| **doorbell** | a write that says only this: where a cursor now is. |

**laws**

> **9.3** memory has two shapes. the ring is time. the region is space. *(picked: a design, signed by the tree. the receipt below shows the ring shape already shipping.)*

> **9.4** the bounds are unrepresentable, never tested. *(derived: from the two definitions above. a cursor with no setter cannot be put outside its ring, and a position of the wrong width is another record.)*

> **9.5** an absence is the one thing that cannot be added later. *(derived: a word can be added to a vocabulary at any time. a word already in it cannot be removed from the programs that use it.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| memory safety is runtime tests and protection faults. | a hosted machine, where the host catches the fall. |
| rollback undoes a write. | a store that rewrites in place and saves the old value so it can put it back. |
| disk and memory are two different things. | their delays, which differ by orders of size. |

**receipts**

a chip: nvme drives are driven through a submission queue, a completion
queue and a doorbell register, each queue a ring of fixed records *(the
field's, from memory)*.

a tool: a ring buffer between one producer and one consumer. each side
advances only its own cursor, and write minus read says how much waits.

**run it again**

no count here.

## 9.4 the walker

*the poke: what does the machine run?*

one piece of code. the walker reads a record, applies a table, and
advances. everything else is data: the records, the rings they stream
through, the walks, the rows that bind a ring to a walk, the tables for
each device. no repeat is written as code anywhere. a ring is a cursor
acting and a cursor moving, over data that carries its own extent.

the walker is an office, in file 5's sense: the one who walks. on the
right chip it becomes the chip. the emulator is the walker pronounced in
a two-valued chip's instructions, built to disappear, and when it goes
these go with it: the packing of each trit into two bits with one state
wasted, the gate tables run as lookups, the inverter, the flags, and the
clock as separate machinery. the flip is two wires crossed (file 4).

anything drawable is DC (file 2), and the machine keeps that split in its
own terms. a drawn, frozen form is fine in the emulator. in the vocabulary
it is fatal, since an absence cannot be added later. so the data is built as if the
chip existed, and the emulator eats the difference until it does.

the walker keeps no gates. it moves values in and out of memory and keeps
one subtraction, differ. every gate is a table it reads, and the
arithmetic unit is a tree of tables of nine entries and one ring.

the lean replaces the branch. on a usual chip an if is a compare and then
a jump: the decision is made in code, and made again on every pass. here
the outcome of the compare is a trit, and the trit indexes a table of
data: a select, and no jump. the ifs go into
data, as rows of a binding table: when this ring has records, run that
walk. a row is taught once. the first time is a conversation with the
programmer, and every time after is a table read.

the walker never goes back. a rewind cannot be spelled. what was written
stays written: the trace only appends, a change is a name laid over the
trace, and undo is that name taken off. this is why rollback undoes no
write. the vocabulary has no word for undoing one.

and a walk stops because its ring does. the walker only advances, one
lap forward visits every slot, and a walk stops at a 0. so a walk that
cannot go back and cannot write into its own ring reaches the ring's 0
within one lap. take one leg away and the guarantee breaks. over every
walk of the first walker that goes round at all (runs E59 and E62):

| what was allowed | walks that never end |
|---|---|
| a ring with no 0 | 45.84% |
| rewinding | 6.24% |
| a walk writing into its own ring | 0.06% |
| none of the three | 0 of 110,808 |

*(measured: in an earlier build, on the tree's own record; not re-run for
this text.)* the three legs are enough, and not each of them is needed:
most walks that write still end. the return is what lets a walk come
home.

**terms introduced**

| term | here it means |
|---|---|
| **binding** | one row of data that says: when this ring has records, run that walk. |
| **binding table** | every binding of a machine. it is where the ifs of a usual program go. |
| **trace** | everything written, in the order it was written. it only appends. |
| **to advance** | said of a cursor or of the walker: to go on to the next slot. it has no opposite. |
| **to teach** | to write a binding. |

**laws**

> **9.6** the walker reads a record, applies a table, and advances. everything else is data. *(picked: a design, signed by the tree.)*

> **9.7** the one code written is built to disappear. *(picked: the emulator stands in for a chip that does not exist yet, and is deleted when one does.)*

> **9.8** the programmer teaches. the walker runs. the ifs are rows. *(derived: from law 9.6 and file 4's lean. a three-way outcome used as an index needs no branch.)*

> **9.9** a walk that cannot go back and cannot write its own ring ends at the ring's 0 within one lap. *(derived: a position that only advances visits every slot of a circle in one lap.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a program is code that branches. | the emulator, which pronounces the lean as a compare and a jump. |
| undo puts back an earlier state. | a machine that overwrites, and so must save what it would lose. |

**receipts**

a chip: x86 already names the pieces. `xor r,r` is the check, zero made
by self-difference. `neg` is the flip, and `not` is not. `mov` is the
wire. `sub` and `cmp` are differ (files 4, 7 and 8).

copper: null convention logic runs on two-valued silicon with no clock,
and crosses two wires for the flip (file 4). part of what the emulator
sheds has already shipped.

a tool: a write-ahead log. changes are appended, and the state is what
the log says when it is read forward.

**run it again**

law 9.9 runs on paper. draw a circle of n slots with a 0 in one of them,
and a position that goes forward one slot at a time and may not write.
it meets the 0 in at most n advances, from any start.

the four percentages are measurements of an earlier build, and are not
re-run here.

## 9.5 the record

*the poke: what is an instruction?*

an instruction is a record, and a record is a coord: n trits, each low,
the return or high, with no fourth state and no absence.

| trits | coords |
|---|---|
| 1 | 3 |
| 2 | 9 |
| 4 | 81 |
| 8 | 6,561 |
| 16 | 43,046,721 |

at two bits to the trit, sixteen trits fill one 32-bit register exactly.
as one number they take less: 3 to the 16th is far below 2 to the 32nd. more trits on one record tell more apart. more records side by
side is throughput. the two are never one move.

the grade (file 3) is how many trits are off the return. the record with
every trit at the return has grade 0, and a corner (file 8) has every
trit at a pole.

a coord is the shape of a compare's outcome, and never a way to store.
in the first walker the only three-valued thing running was the outcome
of a compare, and the stored values were plain integers *(measured: in
an earlier build, on the tree's own record; not re-run for this text)*.
three values belong to comparing, not to storing: trit-typed storage is
never built. in the emulator a record is kept as one plain integer, its
name below. the three values are how a record is read, slot by slot, and
what a compare gives.

the name is the sum. in the third codec of file 2, 0 for the return, 1
for low and 2 for high, with the places 27, 9, 3 and 1, a record of four
trits has a number for a name, and no lookup is needed:

    (+, 0, 0, 0)    54
    (0, 0, +, 0)     6
    (0, 0, 0, +)     2
    (+, 0, +, +)    62    the three together

a table in an earlier build once printed 71 for the last. it had written
the unused second slot as low where the sum keeps the return: 62 and 9.
a missing slot written as a value is another record, and one sum caught
it.

a 0 in a slot is a reach unspent, file 5's held middle. of the 81 records
of four trits, 16 are corners and 65 keep at least one 0. a corner is
complete at one Self and runs here. a 0 that the binding leaves for
another Self makes the record a protocol: it is chained forward unread until that Self finishes
the reach.

the forces, the moves a record orders, by price (file 4):

| price | force | what it is |
|---|---|---|
| paid | the step | a cursor advances by one, and an arrival is read |
| paid | the call | a linkage is sunk, and it must come back |
| free | the flip | the turnaround: each value to its other side |
| free | the compare | on the ring of three it forgets no difference. on the line it forgets at a pole, and that pays |
| free | the pass | the wire, unmarked |
| data | the landings | high, low, and the landed 0 |

the price can be read off the text of a walk: one landing per step, one
linkage per call, none per flip. no profiler is needed.

a record carries no literal. its values arrive from an operand or from
the world. no gate mints a constant from the return (file 8), and no
record carries one: both ways are shut, and every value comes from the
world.

a record has two sides. the opcode is on the page: which force, on which
slots. the operand is supplied by the caller, when the word ends (section 9.7
walks that moment). so a walk is spelled and never looked up, and the
row that says how the caller supplies its side is the calling
convention. file 12 walks writing systems that have always worked this
way. which glyph stands for which opcode is a pick, it is maxi's, and it
is not made: no glyph of this language exists yet.

**terms introduced**

| term | here it means |
|---|---|
| **coord** | a record taken as a position: n trits, each low, the return or high. it is also what addresses a slot of a memory region. |
| **held zero** | a trit left at the return in a record: a reach unspent, left for whoever can finish it. |
| **committed** | said of a slot: off the return, at a pole. |
| **linkage** | the note of where a call must come back to. |
| **protocol** | a record with a held zero. another Self finishes it. |
| **force** | a move a record orders. |
| **step** | the force that advances a cursor by one. paid: it lands. |
| **call** | the force that goes into a region and must come back. paid: a linkage. |
| **literal** | a value written inside an instruction. a record has none. |
| **opcode** | the side of a record that is on the page: which force, on which slots. |
| **operand** | the side of a record the caller supplies. |
| **caller** | whoever runs a walk and supplies its operands. |

**laws**

> **9.10** a record's name is the sum of its slots under a declared codec. *(counted: the four sums, below.)*

> **9.11** a corner runs here. a held zero sends across. *(picked: a design. a 0 is a reach unspent, and the binding says who spends it.)*

> **9.12** the price is a property of the move. steps vectorize. calls serialize. *(derived: from file 4's price. records side by side each land once and wait on no one; a call must come back before the next begins.)*

> **9.13** a record carries no literal. every value arrives from an operand or from the world. *(picked: a design, to match file 8, where no part mints a value. the tables and bindings are data, and they are written by a programmer.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| an instruction set is a list of opcodes to memorize. | the two-valued pronunciation. here a record is composed of slots, the way a word is composed of letters. |
| a constant is written into the instruction that uses it. | a chip whose gates can make a value from no input. file 8 counts why three-valued tables that keep the return cannot. |

**receipts**

a chip: every instruction of every chip is already an opcode and its
operands. x86 leaves the three outcomes of one compare in its flags
(file 4).

arithmetic: 3 to the 16th is 43,046,721, and 2 to the 32nd is
4,294,967,296.

**run it again**

the name. take a record of four trits. write 0 for the return, 1 for low
and 2 for high. multiply the four digits by 27, 9, 3 and 1, and add.
(+, 0, 0, 0) gives 54, (0, 0, +, 0) gives 6, (0, 0, 0, +) gives 2 and
(+, 0, +, +) gives 62. writing the second slot of the last as low gives
71. all 81 records give 81 different numbers, 0 to 80.

the corners. list the 81 records of four trits and count those with no
0: 16. the other 65 keep at least one. at widths 1, 2 and 3 the records
that keep a 0 number 1, 5 and 19.

## 9.6 the fill

*the poke: how does the next thing know it is next?*

nobody tells it. the next thing is whichever ring has fill above zero,
and fill is the reader's own subtraction, write minus read. time is taken
off records, never off the world: order is causal, a count of landings,
and a clock on the wall would put into one order things that never
touched. a stamp is set by the ring at the write, never by the writer.

four things, and no scheduler.

    the gauge    a walk drives until its count is 0: burn until empty.
                 the 0 it stops at is a held zero, a reach this Self
                 cannot finish
    the next     the next thing is whichever ring has fill above zero
    the order    which ring drains first is the treatment order:
                 priority. data the gavel writes, and never computed
    the fuel     what one lap leaves over is what the next lap starts with

the whole cycle of the OS: wait for the doorbell, drain the rings in
treatment order, run the walks their bindings name, wait. there is no
tick. the scheduler is a table read.

a deadline is fuel. the machine has no timeouts: things run out. a
deadline is an amount of fuel raced against a call, and the compare says
which landed first.

priority is the one positive decision no structure dissolves. code that
picks it is the axiom's move of law 1.13 in a scheduler's coat: a pick
that forgot it was picked. written as data and signed by the gavel, it
stays a pick.

two Selves go one after the other the same way: whoever fills first
writes next. the order falls out of the fill, and no one schedules it.

a ring that swings between full and empty is not too shallow. depth buys
only a burst, and with unequal average rates no depth is enough.

**terms introduced**

| term | here it means |
|---|---|
| **gauge** | a walk's count of what it has left to burn. the walk runs until its gauge is 0. |
| **fuel** | what one lap leaves over, which the next lap starts with. |
| **priority** | which ring drains first. a row of data. |
| **treatment order** | the rings, listed in the order they drain. |
| **the gavel** | the say over a machine's priorities, and whoever the machine belongs to, who has it. the gavel writes priority, and no code computes it. |
| **stamp** | the place in the order that a record is given when it is written. the ring sets it. |
| **deadline** | an amount of fuel raced against a call. |

**laws**

> **9.14** no one is told when to run. each one reads the fill. *(derived: from section 9.3. fill is the reader's own subtraction, and it needs no one else.)*

> **9.15** priority is data the gavel writes. code that picks it is the axiom's move. *(derived: from law 1.13. a pick written as code has lost its signature.)*

> **9.16** a ring that must be deep is a flow that is wrong. redesign the flow. *(derived: depth keeps one burst. unequal average rates fill any depth.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a scheduler decides who runs next, on a timer. | a machine that pretends one walk sits at two clocks. |
| a timeout is a limit on waiting, kept by a clock. | a clock outside the work. here the limit is fuel, and it runs out. |

**receipts**

computing: lamport (1978) ordered the events of a system by what could
have caused what, and never by a shared clock. events that never touch
stay unordered in that relation *(the field's)*.

a tool: a ring shared by one writer and one reader, such as io_uring's
completion queue. whoever takes from it subtracts its own cursor from the
writer's to learn whether any record waits.

**run it again**

no count here.

## 9.7 the close

*the poke: when does anything fire?*

at the close. type t, h, e. what was typed is not known yet: the next
key may make it then, there or theory, or a space may end it. a response
per letter would respond to a word that does not exist. so the letters
stream in free, and the machine binds and responds once, at the
boundary.

the organ that does it is a capacitor with a threshold on it: integrate,
compare, fire. each arrival adds to the charge. a threshold compares the
charge against the boundary. at the close a switch fires and discharges
it, and the return is made again (file 7). fill is the charge: write minus
read, zero when empty, full at the lap. a capacitor's voltage is the sum
of every current that arrived.

charging is free: below the boundary the test runs per letter and
commits no response. firing is paid: an offer landing. a letter that cannot
extend the word resets for free, the cursor simply not advancing. hold,
fire, drop.

and one press is one move. a key that composes a flip with a step hides
both the price and the order. keep them two moves, the free one and the
paid one, and the hands feel which is which.

there is no send key. politeness is differ on the other's fill: while
their word is still charging, my full capacitor keeps its charge.
interrupting is discharging into their unfinished word. two writers
driving one wire at once is the same tear, built in.

the scene that made it land. I am typing a post in a browser, the music
stops, and mid-post I type the words for next track. the presses charge
a capacitor that sits between the keyboard and every program, and no
letter fires. at the boundary there is one read, and the record lands in
the music's ring. the browser's ring got no letter, and no letter was
deleted from it, since none ever landed there. a page can only name what
reached it.

the read at the close is a fold (file 7). where I stand after a word is
where I stood, minus the tally of what arrived. between closes, forms
compose unread, and the brackets they carry record which walk was gone
through, never an order of operations. in file 7's notation, (0 to 1) to
2 and 0 to (1 to 2) are two walks, landing 0 and 1, and only the close
says which was walked.

that read is the one move that loses anything, and it runs once per
word. file 7 found three doors landing on every digit, and the digit
keeping none of them. so the doors are shipped, and the fold is taken
only where a word ends.

the calculus has a theorem of this shape. sum a finished walk's leans,
and every middle landing, written once arriving and once leaving,
cancels. only the ends are left: where I am, minus where I began.
double-entry books net their inner transfers to zero the same way.

in a long string the 0s are the walls: they split it into rooms, and the
runs between them are the words. fold each room, and a room that lands
at the return becomes a 0 one scale up: the carry of file 6, in the
string.

a stream with no close marked in it leaves the cutting to its reader, as
unspaced scripts do. this machine carries its close inside the stream.
english carries it as the space: silence, written as a mark.

a close can tear across two clocks. a cursor shipped as a number can be
torn by a whole word: from 222 to 000 every digit changes at once.
shipped in gray code, where one digit changes per advance, a torn read
loses one advance at most. this is why queues between two clocks send their
cursors in gray code (file 7).

a watcher is a third cursor, one that only reads. its own tally of my
marks charges until it matches a walk it has seen, and then it fires a
completion. autocomplete is the caller's side of the record, run ahead
of the caller.

a completion that writes itself into my stream is the machine supplying
my operand, and auto-commit is that fault shipped as a feature. an offer
narrows the menu instead: every letter I spell is one more constraint,
and when what is left fits a screen, the menu appears and I pick from
it.

every watcher gets an offer ring of its own, since completing straight
into the walk would be two writers on one wire. which offer lands is the
gavel's pick or priority data, never computed.

**terms introduced**

| term | here it means |
|---|---|
| **close** | the end of a word, where the machine binds and responds, once. |
| **boundary** | the mark or the level that says a word has ended. |
| **capacitor** | the organ of the close: a part that adds up arrivals, with a threshold that compares the total against the boundary and a switch that fires. named for the part that does the adding. |
| **word (the machine's)** | the records that arrive between two closes. |
| **charge** | what a capacitor has between closes. it is performed, and never shipped. |
| **the torn read** | a read taken before the close, or taken while a second writer is on the wire. |
| **watcher** | a cursor that only reads, and fires a completion when what it read matches a walk it has seen. |
| **offer** | a completion laid before me, to pick or to leave. it never writes into my stream. |
| **auto-commit** | a completion that writes itself into the stream. |

**laws**

> **9.17** no letter fires. the boundary is the send. *(walked: the poke above. a response per letter responds to a word that does not exist yet.)*

> **9.18** fold only at the close. brackets are the trace, never precedence. *(counted: the two bracketings, below.)*

> **9.19** a watcher's completion lands as an offer, never as a write into my stream. *(derived: two writers on one wire tear, so a watcher writes only to a ring of its own.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| an input is handled the moment it arrives. | a machine that responds per letter: the torn read. |
| brackets say which operation goes first. | sums and products, where regrouping changes no result. the fold is a subtraction, and regrouping it lands somewhere else. |
| autocomplete saves typing by typing for me. | auto-commit. an offer saves the typing and leaves the pick with me. |

**receipts**

copper: a capacitor. the books on neurons give the same three acts one
name, integrate-and-fire *(the field's, from memory)*.

a tool: a unix terminal, as it comes, keeps the keys and delivers the
whole line at the newline. programs behind it never see a letter alone.

a chip: a queue between two clock domains passes its cursors in gray
code, so that a read taken mid-change is off by one slot and never by a
word *(the field's, from memory)*.

**run it again**

the two bracketings. on the ring of three, x to y is x minus y taken
round the ring. (0 to 1) to 2 is 0 minus 1, minus 2: minus 3, which is 0
on the ring. 0 to (1 to 2) is 0 minus (1 minus 2): 1.

the tear. count from 222 to 000 in base 3: three digits change in one
advance. now write each count in gray code: read its digits highest place
first as the stands of a walk that starts at 0, and take each stand minus
the next, round the ring. 222 becomes 1 0 0 and 000 becomes 0 0 0: one
digit changes. the same holds at every one of the 27 advances.

## 9.8 the arena

*the poke: how long does a thing stay in memory?*

two lifetimes, two mechanisms. regions are carved once at start-up, last
long, and are reset cold. what churns is ring records: letting one go is
the cursor moving on, its slot is used again at the next lap, and a
stale reader is one that fell a lap back, caught by the same subtraction
that tests for a full ring.

each ring's policy for overflow is set when the ring is made.

    block   for commands, where losing a lap is not allowed
    drop    for input and display frames, where the stale is worthless
    kick    to protect the system from a watcher that stopped taking

the policy is a choice only while the average rates are equal. with
unequal averages no depth is enough (law 9.16). the averages are made equal
by one trick under four names, batching, coalescing, moderation and
chaining: rate-shaping. a ring that drops runs an inward spiral, and its
drift is what it dropped.

there is no heap. everything is carved at start-up: one arena, a table
of regions, regions claimed by a bump and never given back, records of
fixed width. unbounded data streams through a fixed ring. five
guarantees sit in the instruction set itself:

    time        the cursor has no setter, so no cursor leaves its ring
    space       no coord exceeds its span
    lifetime    a stale handle cannot be used
    ownership   one writer per region
    isolation   no raw address in the vocabulary, so no walk reads
                wherever it likes

and sharing has no order of its own. several writers into one record are
sends on one wire, and the medium sums them at once (file 4): nobody
performs the sum, and the world gave the writers no clock to put them in
order. so a shared record sums on the ring. each write advances the
digit, a full column carries into the next (file 6), and the record is
read once, at the close. every order of the writes lands on the same
total. the one loss is that read, when the carry has no column left to
go to. this is a claim about order. each write must still land whole: two
adds that tear each other are the torn read of section 9.7, and the build has to
rule them out by other means.

two-valued machine words already run it. a sum that carries round the
register is exact in every order whenever the final total fits, since
adding round a register gives the same total in any order and any
grouping.

the cheap sum clips at the poles: high plus high stays high. it reads at
every write: a forgetting per arrival, a fold taken before the close.
that early read is what puts an order into the writers.

| writers | sets of summands | sets whose order changes the clipped total |
|---|---|---|
| 2 | 6 | 0 |
| 3 | 10 | 2 |
| 8 | 45 | 27 |

two writers never depend on their order. three do, one set in five.
eight do, three sets in five.

absence also ends the early outcome. a walk that tests records cannot
read the ring its outcomes go to: whoever takes from that ring is on the
far side of a seam. so the walk cannot act on an outcome early. the
early act is not forbidden. it is unrepresentable, the way a function
with no write in its address space cannot have a side effect.

**terms introduced**

| term | here it means |
|---|---|
| **arena** | all the memory of the machine, carved once at start-up into regions and rings. |
| **policy** | what a ring does when it is full: it makes the writer wait, it lets the oldest record go, or it cuts off whoever stopped taking. set when the ring is made. |
| **rate-shaping** | making two average rates equal: batching, coalescing, moderation, chaining. |
| **stale** | said of one that fell a lap back on a ring, or of a handle to a region that was reset. |
| **the cheap sum** | a sum that clips at the poles, and so reads at every write. |

**laws**

> **9.20** shared writes sum at once. only a read before the close makes their order matter. *(counted: the clipped sum, below. the exact half is proved by machine in sibarum/cott-lean at commit 025897b, `Scatter.read_exact`.)*

> **9.21** safety sits in the vocabulary: time, space, lifetime, ownership and isolation each stand because the fault cannot be written. *(picked: a design, on laws 9.4 and 9.5. the mechanisms for lifetime and ownership are not designed yet.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| programs ask for memory as they run and give it back when done. | a heap, and the faults that come with one. |
| shared data needs a lock to put its writers in order. | a store that is read and rewritten at every write. a sum read once needs no order. |

**receipts**

a proof: in sibarum/cott-lean at commit 025897b (2026-09-25),
`Scatter.read_exact` shows that a
register of w bits that carries round, taken as signed, has the exact
total whenever the final total fits in w signed bits, whatever the
partial sums did; `Scatter.run_perm` shows that every schedule of the
writes gives one result *(the field's: proved by machine in lean 4. the
commit is named because these proofs have since left that repository's
head)*.

a chip: addition in two's complement carries round the register, and is
exact in any order while the total fits.

**run it again**

the clipped sum. take the three values minus 1, 0 and plus 1. for n
writers, list every set of n summands, repeats allowed and order
ignored: 6 sets for 2 writers, 10 for 3, 45 for 8. for each set try
every order: start at 0, add each summand, and after each add clip the
total into the span from minus 1 to plus 1. a set depends on order when
two of its orders end on different totals. expect 0 of 6, 2 of 10 and 27
of 45.

then replace the clip with a sum that carries round a register wide
enough for the total, and take the total once at the end. no set depends
on order.

## 9.9 the forces

*the poke: what does a record order, and what can it not say?*

moves. a record's slots are its forces, and section 9.5 sorted them by price.
whether anybody owes a 0 is a fact of the binding, not of the opcode: a
record with one slot high and three at the return runs alone and owes no
one. what the coord does say is where a reach can be finished: a corner
runs here, a held zero sends across. a held force does not stall the
walker. the walker binds, chaining the record forward unread, and the
reach is finished at whichever Self supplies it. a walk that would wait
is two walks with a ring between them.

a touch on a region is a call in another dress: a request, with its coming
back owed. and direction is a role: reader and writer make the same
contact, and which one I am decides take or leave. file 7 found
direction worn at the ends and never in the record, and the machine
keeps it there: in the binding, never in a digit. the forces follow the
shapes of memory. rings give the step, regions give the call, and the
free moves ride either shape.

no slot is ever missing. low is a value. an earlier build stalled for
months on one notation that wrote forces and coords alike and took the
low mark to mean "absent". two structures that agree on every count and
differ on what the digits mean are told apart by no counting.

the chip already knows the price belongs to the move. x86 fused a
handful of compositions into single instructions, the move of a run of
bytes, the store of a run, the scan, the compare and the counted repeat,
and not one of them contains a call. and a vector register runs several
records under one instruction pointer: more than one where, and one
when, since there is one walker.

in the earlier build, the emulator's own cost was its mispredicted
branches and its bytes, never its count of instructions: the encoding's
cost, not the move's. a walker that branched on the grade was built, and
it ran slower than one table for every grade. a three-way partition
written in x86 took eleven instructions per item, six of them routing
and three of them jumps deciding again what the compare had already
settled. the table took four *(measured: in an earlier build, on the
tree's own record; not re-run for this text)*.

what cannot be written:

    a read and a write of one slot   the record with every trit at the
    at once                          return is a turnaround, and one
                                     digit cannot say both ways
    the chair, in ink                the zero the page never keeps
                                     (files 3 and 7)
    a write that never lands
    action at a distance             no move reaches a slot it does not
                                     touch
    an input left floating           every wire needs its pull
    a cursor set to a position       it has no setter
    a step across two grades         one step commits one slot

x86's `xchg` tries the first of these, a read and a write at once, and
pays with a lock it cannot drop. the fault is priced there. here it
cannot be said.

**terms introduced**

| term | here it means |
|---|---|
| **role** | reader or writer at one contact. a fact of the binding, never a digit of the record. |
| **contact** | where a record touches a ring or a region. |

**laws**

> **9.22** direction is a role: a fact of the binding, never a digit of the record. *(derived: from file 7. direction is worn at the ends, never in the record.)*

> **9.23** one step commits one slot. a corner is reached only through a pole. *(derived: from section 9.5 and file 5's count of moves. every move changes one slot.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a missing value is written as zero, or as minus one. | a format with optional fields. here every slot has one of three values, and none of the three means missing. |
| to read and write one place in one instruction is a feature. | x86's `xchg`, which locks every time it touches memory. |

**receipts**

a chip: x86's `rep movs`, `rep stos`, `repe scas`, `repe cmps` and `loop`
are five such fused compositions *(the field's)*.

a chip: `xchg` with a memory operand is locked without being asked,
whether or not the lock prefix is written *(the field's)*.

**run it again**

no count here. the instruction counts and the slower branching walker
are measurements of an earlier build.

## 9.10 the driver

*the poke: what stands between two clocks?*

a driver. across a seam with one clock, parts compose and no thing
stands between them. across a seam with two clocks a driver is required:
one record spans the two clocks, and no walk does. a blocking call is
the fiction of one walk sitting at two clocks at once, and threads,
context switches, schedulers and async are the price of that fiction.

this gives unix's "do one thing well" its size: one Self's work between
two seams. fuse whatever contains no call inside one Self. split at a
call, at a change of clock, or at another Self.

what crosses between the two clocks is the arrival, never the stand
(file 7), the way the close ships its cursors in gray code.

a driver is two tables.

    the format map   coord to the device's bytes: the datasheet,
                     transcribed
    the rate shape   fill to batch size: all rate-shaping in one table

the only thing it reads while running is fill. a paint brush is one: a
map from the gesture, which carries to any screen, into one screen's own
bytes.

the spec sheet is the other Self's language, kept whole at mine. a
driver is quotation: one Self's write carried whole inside another's. it
sits at a held zero, where a second Self finishes the reach. firmware is
signed by its vendor, and neither end runs the other's code. only shared
records and a doorbell cross, and a completion landing is the other
Self's write finishing my held zero.

format compatibility is the dial (file 4) at a seam. the same format is
matched, and the record is taken. a different one is not taken: what the
far side makes of it is garbage, and no error says so. records are never
converted between rings: they match, or they do not. a driver's format
map is the one place a record is rewritten, and it stands at a device,
never between two rings.

finding the match is the expensive search, paid once. keeping the match
is cheap. a driver is the certificate of a finished search: the witness,
which is the complexity books' word for what lets a hard search be
verified in easy time. learning is the same thing at a Self: a found way
getting a name, paid for once and kept.

the driver and the capacitor are one thing with two faces. the driver is
the capacitor bare: the table, transcribed, shippable, with no charge.
the capacitor is the driver powered: the fill rising, performed at a
Self, never shipped.

a driver never names its trigger. it reads a ring, and whatever writes
that ring is the user's wiring, one row. its output lands on its own
ring as an offer, never as a write into anyone's stream. the wiring
diagram is the permission model.

the machine meets its own two clocks the same way. the assembler writes
the walker at build time and the chip runs it at run time, and the
executable is the one record that spans both. the processor is a device,
and the walker is its driver. compiling ahead and compiling just in time
are one function, and the second sees the fill.

**terms introduced**

| term | here it means |
|---|---|
| **driver** | two tables at a seam between two clocks: a format map and a rate shape. transcribed from a spec sheet, never written. |
| **format map** | the table from a coord to a device's bytes. |
| **rate shape** | the table from fill to batch size. |
| **matching network** | what a driver is at a seam: what makes one side's format matched to the other's. the radio engineers' word. |
| **witness** | the certificate of a finished search: what lets a hard search be verified cheaply. |
| **quotation** | one Self's write carried whole inside another's. |
| **blocking call** | a call that waits on another clock. |

**laws**

> **9.24** one record spans two clocks. one walk never does. *(derived: from file 2's clock and law 9.14. a walk's order is its own count of landings, and two clocks share no count.)*

> **9.25** a driver is transcribed, never written. *(candidate: from section 9.2. no driver has been transcribed yet.)*

> **9.26** a driver is the matching network. *(derived: from file 4's dial. at a seam a format is matched and taken, or it comes back.)*

> **9.27** a driver is a finished search, held cheap. *(derived: from what a witness is. found once at full cost, verified cheaply ever after.)*

> **9.28** a driver can be given. a charge cannot. *(derived: from section 9.7. a table is ink and ships. a charge is performed at one Self.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a driver is kernel code, written per device. | a machine whose drivers were compiled and frozen months before the device they face. |
| a blocking call waits for the device. | one walk pretending to sit at two clocks. |
| knowing is a store of facts. | a driver: a found match, kept cheap. |

**receipts**

a datasheet: the register map of any device is already a table from
meaning to bytes. a driver written by hand restates it in code.

complexity theory: a certificate lets an answer that was hard to find be
verified quickly *(the field's, from memory)*.

copper: a matching network between a transmission wire and an antenna
does for a wave what a driver does for a record (file 4).

**run it again**

no count here.

## 9.11 the metal

*the poke: what is this built from, and does it carry over?*

every decision is weighed by that one test, and never by what makes the
hosted version fastest. the hosted machine is the workshop, never the
product, and the urge to ship a quick working version is a habit to
catch. every touch of the host wears a numbered note saying how it
dissolves when the host is gone, and those notes are the complete list
of what the port has to do. this is the build's fiat: signed by the
tree, arguable, kept in place.

the phases peel one seam each.

    guest    the machine draws as a window on the host
    owner    linux runs headless under it as the net, while the machine
             takes the graphics card raw
    metal    started from a thumb drive: only the device list, the memory
             map and the start-up change

the interface survives every phase, and drivers written over the raw
rings carry to the metal nearly whole.

a host's driver is mostly two things: defensive code against impossible
states, which a walk that never rewinds makes evaporate, and the kernel
as referee between programs, which rings and counts replace. what stays
is thin: power states and real faults. signed firmware is the vendor's
real chokepoint: a sequence of register writes cannot be shut away, and
a blob can. "pages arrive zeroed" is a host's fact promoted to a
guarantee, and it dies exactly where no one can debug it. such a
dependence gets a note.

every hardware border is one pattern. the data does not vary: the walk,
the draw record, the input record, the stored record. the hardware
varies under it. the seam is designed once. everything per device is
data: one walker and a table per device, brought together only at
dispatch, and never an object per device with its own detect, init and
run.

a count is general, and a layout of bits belongs to the platform: if two
platforms make me write it twice, I wrote the mechanism. the framebuffer
is a ring, and showing the next frame is a cursor advance: one
vocabulary of draw records, and one small table per card translating it,
with the processor drawing when no card responds.

two conditions, maxi's, never softened.

    1   the machine is never the only thing between maxi and his
        keyboard. taking a device needs a way back that is not that
        device: a second input, a remote shell, a serial wire
    2   one driver per stack. his daily keyboard stack is never touched.
        the machine observes only, until a written list of conditions for
        taking input has been earned

the chip's own start is the check (file 7). at power-on the chip begins
at an address fixed by its design, the reset vector, and the firmware
found there runs a self-test. which edge comes first is a pick, and the tree picked
the fall before the rise.

and the substrate. a chip's instruction set is a sequential face over
dataflow over analog physics. the dataflow machine won decades ago and
was put behind an old interface. the cheap test is a field-programmable
chip: the same physics, and no instruction set at all. walks that run
there with no walker translating them would show that the limit was the
interface.

**terms introduced**

| term | here it means |
|---|---|
| **the metal** | the machine started with no host under it. the product. |
| **guest, owner** | the two phases before the metal: a window on the host, then the host kept only as a net. |
| **port** | the move from host to metal. its whole content is the numbered notes. |
| **substrate** | what a chip is under its instruction set: dataflow, over analog physics. |

**laws**

> **9.29** linux is the bootloader. the metal is the product. *(picked: the build's fiat, signed by the tree. the other choice is to ship the hosted version.)*

> **9.30** state the law, never the mechanism. a platform difference is never a design fork. *(derived: from sections 9.3 to 9.6. a count carries to every platform, and a layout of bits is one platform's.)*

**the usual reading**

| the usual reading | where it holds |
|---|---|
| a new architecture waits on new hardware. | the physics. the limit is the interface. |
| ship a quick working version first. | a product that stays on its host. |

**receipts**

a chip: every processor begins at an address fixed by its design, its
reset vector, since at power-on no program exists yet to say where to
begin *(the field's)*.

a chip: an out-of-order core already runs dataflow under the old face.
an instruction issues when its operands arrive (tomasulo, 1967) *(the
field's, from memory)*.

**run it again**

no count here.
