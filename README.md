# Rexgen 

This is a simple string generation library for Rust code. It only supports some simple regular expressions

## Example

```rust
//for reuse example
for _ in 0..15 {
        let gen = RegexGenerate::max_repeate(10).parse(r"\d{3}-\d{8}|\d{4}-\d{7}",20);
        println!("{}", gen.generate());
}
/** 
 * out:
 * 296-33838069
 * 8765-4739082
 * 454-79535302
 * 9039-2273160
 */


```
or
```rust
// for one-time use
let a = regex_gen("\\w+@(abc|efd|xyz)\\.com",20);
println!("{}", a)
// out: vCqf@abc.com


```
