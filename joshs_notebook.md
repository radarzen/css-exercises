## Why `margin: 0px auto;` centers a block-level element

**Question:** What about the "auto" statement in `@style.css` button style makes it move to the middle of the screen versus being on the left without it?

**Answer Summary:**

The `margin: 0px auto;` declaration, specifically `auto` for the left and right margins, horizontally centers a block-level element within its parent container. This works due to three key factors:

1.  **`display: block;`**: The element (in this case, the button) must be a block-level element. Setting `display: block;` for the button ensures this.
2.  **Explicit or Intrinsic Width**: The block-level element needs a defined width that is less than its parent's width.
3.  **`auto` Margin Behavior**: When `margin-left: auto;` and `margin-right: auto;` are applied to a block-level element with a constrained width, the browser distributes any *remaining* horizontal space within the parent container equally to both the left and right margins. This equal distribution effectively centers the element.