# server_generator_mod
Derived from v2 of `api_gen`.

`api_gen` is a library specialized for `Monorepo`.
If you want to manage your project based on a `multi-repository`, the library may not generate code correctly due to the different directory structure.

`server_generator_mod` solves that problem and helps to manage projects with a directory structure like the following:

```bash
./
├── Makefile
├── api
│   ├── account
│   │   ├── cards.go
│   │   ├── connect
│   │   │   └── login.go
│   │   └── profile.go
│   ├── apigen
│   ├── get.go
│   ├── items/
│   ├── items.go
│   └── users/
├── cmd
│   └── main.go
├── domain
│   └── model
├── go.mod
├── go.sum
└── pkg
    ├── firebase
    └── validator
```

# api_gen
[https://github.com/go-generalize/api_gen](https://github.com/go-generalize/api_gen)