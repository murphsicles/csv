# @encoding/csv — CSV Parsing for Zeta

Auto-converted from [csv](https://crates.io/crates/csv) v1.4.0 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
- **Reader** — configurable CSV reader with flexible record handling
- **Writer** — CSV writer with quoting, escaping, and delimiter configuration
- **Flexible records** — access by index or header name
- **Serde integration** — deserialize rows into typed structs
- **Byte records** — zero-copy record access
- **Configurable** — delimiter, quote character, escape character, comment, headers, flexible length

## Usage
```zeta
use @encoding/csv::Reader;

let mut rdr = Reader::from_path("data.csv").unwrap();
for result in rdr.records() {
    let record = result.unwrap();
    println!("{:?}", record);
}
```

## Stats: ~4,666 lines, 0 unsupported items

## License: MIT