---
title: "Style test"
categories: [meta]
---

This post exercises every style used across the site so the CSS can be
verified in one place. Delete it once the design is settled. Here is some
*emphasized text*, some **strong text**, and some `inline code`. Here's
"a double quote", and some em dashes --- like these. Occasionally there's
~~strikethrough~~ too.

Here is [a link](/), and a [`code link`](/).

## A second-level heading

Body text under an `h2`. Long-form paragraphs are set in a serif face at a
comfortable measure, while all of the structural chrome around them stays in
monospace.

### A third-level heading

A C++ code block:

```cpp
#include <cstdint>

// Read a target word, byte-swapping if host and target disagree.
uint32_t read_target_word(const uint8_t *buf, bool big_endian) {
  uint32_t value = 0;
  for (int i = 0; i < 4; ++i)
    value = (value << 8) | buf[big_endian ? i : 3 - i];
  return value;
}
```

And a shell session:

```sh
$ gdb --batch -ex 'info sharedlibrary' ./a.out
$ objdump -d -j .text a.out | head
```

A blockquote:

> Debugging is twice as hard as writing the code in the first place.
> Therefore, if you write the code as cleverly as possible, you are, by
> definition, not smart enough to debug it.

Lists, unordered:

- First item with `inline code`
- Second item with a [link](/)
- Third item

And ordered:

1. Configure
2. Build
3. Swear
4. Rebuild

A table:

| Register | Purpose            | Saved by |
|----------|--------------------|----------|
| `r0`     | return value       | caller   |
| `sp`     | stack pointer      | ---      |
| `lr`     | link register      | callee   |

A horizontal rule:

---

And that's everything.
