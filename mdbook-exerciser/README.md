# exerciser

This is an mdBook renderer to generate templates for exercises from the Markdown source. Given a
Markdown file `example.md` with one or more sections like:

````markdown
<!-- File src/main.rs -->

```rust,compile_fail
{{#include example/src/main.rs:main}}

fn some_more_code() {
    // TODO: Write some Rust code here.
}
```
````

It will create a file `book/exerciser/exercise-templates/example/src/main.rs` with the appropriate
contents.
