---
title: Are we **Ratatui** yet?
author: Samuel "sermuns" Åkesson

theme:
  name: terminal-dark
  override:
    default:
      margin:
        percent: 5

    intro_slide:
      title:
        alignment: center

    slide_title:
      padding_top: 0
      padding_bottom: 0

    footer:
      style: empty

---

<!-- jump_to_middle -->
Yes, I would say so!
---

<!-- end_slide -->
# Who am I?

- Swedish student

    - Final year of M.Sc. Computer Science and Engineering at Linköping University
<!-- newline -->
<!-- pause -->

- Rust enthusiast since 1 year
<!-- newline -->
<!-- pause -->

- **I have a parasocial relationship with Orhun Parmaksız**

<!-- end_slide -->
# The next 5 minutes

<!-- incremental_lists: true -->

- My journey of porting Ratatui
    - ..to the Nintendo Switch
    - ..to PDFs (**ratatypst**)
    - ..to SVG (**ratasvg**)
    - ..to UEFI (**ratatuefi**)

- Other works

<!-- end_slide -->
# Ratatui on Nintendo Switch


- `nx` from `aarch64-switch-rs` project gives Rust binding to homebrew libraries
- `mousefood` gives a Ratatui backend for rendering to bitmap graphics

![](./ratatui-on-nintendo-switch.jpg)

<!-- end_slide -->
# Ratatui in PDFs: _ratatypst_

- Typst is a fantastic alternative to LaTeX (written in Rust btw)
<!-- new_line-->
<!-- pause -->
- You can write plugins in _any language that can compile to WASM_
<!-- new_line-->
<!-- pause -->
- `ratatypst` is my library for creating your own Typst plugins that render Ratatui widgets!
<!-- new_line-->
<!-- pause -->

<!-- end_slide -->
# Ratatui before the OS: _ratatuefi_


<!-- end_slide -->
# Ratatui widgets to SVGs: _ratasvg_

<!-- list_item_newlines: 2 -->
<!-- incremental_lists: true -->

- _Very undercooked..._
- Use Ratatui for graphic design
- I am unsure of how the user experience should be
    - Currently it is meant to be ran in `xtask` (generate your project's banner)
    - Would be cool to have a CLI that scans your codebase for Ratatui widgets and auto-renders them?


<!-- end_slide -->
# My takeaways

- Rust is really portable!
    - But it's much easier working with x86 and ARM (as opposed to PowerPC..)

<!-- end_slide -->
# References

- _https://github.com/sermuns/ratatui-on-nintendo-switch_
- _https://github.com/aarch64-switch-rs_

