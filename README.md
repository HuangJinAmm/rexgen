# Rexgen 

This is a simple string generation library for Rust code. It only supports some simple regular expressions

## example

'''rust
let s = RegexGenerate::max_repeate(10).parse("优秀|良好|及格|不及格").generate();
println!("{}",s);
'''
or
'''rust
        let a = regex_gen("\\w+@(abc|efd|xyz)\\.com",20);
        println!("{}", a)
        // out: vCqf@abc.com
'''
