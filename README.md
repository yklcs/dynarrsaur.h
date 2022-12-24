# dynarrsaur.h

A single header C generic dynamic array ("vector") library 🦖

Mainly for personal use. You probably shouldn't use this.

## Usage

```c
#include "dynarrsaur.h"
// ...
typedef dynarr_t(int) dynarr_int_t;
dynarr_int_t v = dynarr_init();
dynarr_allocate(&v, 16);
dynarr_push(&v, 0);
int first = v.data[0];
dynarr_free(v);
```

## Features

- Single header
- Generic
- Preprocessor abuse!

## TODO

- Tests
- Element deletion
- Error handling
- Better API
