# Wordlist
Susy Brain Wallets wordlist library


[Rust Documentation](https://docs.rs/susy-wordlist/)


# RUST

```toml
# Cargo.toml

[dependencies]
susy-wordlist = "1.2"
```

```rust
# main.rs

extern crate susy_wordlist;

fn main() {
  println!("Words: {}", susy_wordlist::random_phrase(12));

  let phrase = "violin oblivion cylinder list disarray wobbly fastball showplace oasis patronize septic spearhead";
  println!("Valid: {:?}", susy_wordlist::validate_phrase(phrase, 12));
}
```


# JavaScript


```bash
$ npm i @susytech/susy-wordlist --save
```


```js
// main.js

import { randomPhrase, verifyPhrase } from '@susytech/susy-wordlist'

console.log(randomPhrase(12))

// This will throw if the phrase is not valid:
verifyPhrase("violin oblivion cylinder list disarray wobbly fastball showplace oasis patronize septic spearhead", 12)
```

