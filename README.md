# Lexbor

[![Build Status](https://github.com/kostya/lexbor/actions/workflows/ci.yml/badge.svg)](https://github.com/kostya/lexbor/actions/workflows/ci.yml?query=branch%3Amaster+event%3Apush)

Experimental html parser for Crystal based on new lexborisov's HTML5 parser [lexbor](https://github.com/lexbor/lexbor). More faster and cheaper than [myhtml](https://github.com/kostya/myhtml), and replacement for it in future. Usage is pretty similar to myhtml, see examples. Only missing css selectors feature.

## Installation


Add this to your application's `shard.yml`:

```yaml
dependencies:
  lexbor:
    github: kostya/lexbor
```

And run `shards install` (Installation require gcc and cmake, make sure it installed)

