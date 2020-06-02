This is just a short reproduction case for rust issue https://github.com/rust-lang/rust/issues/72933 .


When run with rustc 1.45.0-nightly (ad4bc3323 2020-06-01), this is the output of cargo build:

````
# cargo build 

   Compiling proc-macro2 v1.0.18
   Compiling unicode-xid v0.2.0
   Compiling syn v1.0.30
   Compiling serde v1.0.111
   Compiling quote v1.0.6
   Compiling serde_derive v1.0.111
   Compiling repro1 v0.1.0 (/home/anders/repro_enum_serde_stackoverflow)

thread 'rustc' has overflowed its stack
fatal runtime error: stack overflow
error: could not compile `repro1`.


 ````


