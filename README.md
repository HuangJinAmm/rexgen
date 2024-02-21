# Rexgen 

This is a simple string generation library for Rust code. It only supports some simple regular expressions


## Example

```rust
//for reuse example
//max_repeate(10) means the max repeat times of the string where generate from regex is 10
//max_repeate is a optional parameter, if not set, it will be set to 20
for _ in 0..15 {
        let gen = RegexGenerate::max_repeate(10).parse(r"\d{3}-\d{8}|\d{4}-\d{7}",20).unwrap();
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
