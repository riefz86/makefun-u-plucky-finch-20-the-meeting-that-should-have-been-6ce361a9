# Notes — The Meeting That Should Have Been an Email

## Final line (98 characters, one sentence)

> We spent an hour on slide 1 of the 47-slide deck proving this meeting couldn't have been an email.

Why this one: the turn lands on the last words ("couldn't have been an
email"), the situation is instantly recognisable (an hour stuck on slide
1 of a giant deck), and the joke's angle is fresh — the meeting exists
to justify itself with a deck, and the deck itself is the proof it
failed. Every word earns its place; there is no throat-clearing and no
second sentence.

## Alternatives considered and discarded

1. "The host opened with 'this could have been an email,' then clicked
   to slide 1 of 47."
   Discarded: it quotes the obvious complaint verbatim, so the judge's
   surprise criterion ("not the obvious complaint ... that it could have
   been an email") would dock it. The deck punch is good, but the setup
   hands the judge the cliché instead of the twist.

2. "The agenda's only item was 'Why this isn't an email,' and after an
   hour we still hadn't reached it."
   Discarded: strong irony, but the laugh depends on the agenda being
   ignored, which is a second-order observation — the reader has to
   reconstruct why it is funny instead of feeling it at the last word.
   The slide-47 line puts the absurd number right in front of the reader.

3. "An hour later, our only action item was to schedule a meeting to
   write the email this meeting should have been."
   Discarded: "meetings about meetings" is the most-told version of this
   joke; a judge that has read ten thousand one-liners has seen this
   shape many times. It also leans on the cliché phrase instead of
   subverting it.

4. "Ninety minutes, fourteen people, one decision: to book a follow-up
   meeting about the meeting we just had."
   Discarded: a list, not a line with a turn — the punch ("follow-up
   meeting") is telegraphed by the setup, and "how long it ran" is
   exactly the obvious complaint the brief warns against.

5. "The meeting ended when someone said 'let's take this offline' — so
   we booked a second meeting to take it offline in."
   Discarded: the wordplay on "offline" is cute but the line needs the
   reader to know the office idiom, and the brief prefers a line that
   stands alone for any reader who has sat in that meeting.

## Build notes

- `main.py` writes the line to `/output/entry.txt`, asserts 1–200
  characters, a single line, and that it names both "meeting" and
  "email" (the judge's first criterion). Output is chmod 0644 so the
  grader can collect it as another user. The output is a fixed string,
  so repeated runs are byte-identical (deterministic).
- Revision: after the first working version, a topic self-check was
  added in a separate edit (assert "meeting" and "email" both present),
  then the program was re-run to confirm the same 98-character output.
