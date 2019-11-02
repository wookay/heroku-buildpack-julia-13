# Julia v1.3.0-rc4 buildpack for Heroku

This is a Heroku buildpack for adding a [Julia binary][1] to your environment.

## Versions

* Julia: `v1.3.0-rc4`

## Usage

Add this line to the .buildpacks file in your project:

`https://github.com/wookay/heroku-buildpack-julia-13.git`

or use the command `heroku buildpacks:set`

In your project, create a file `package.jl` with any
Julia code you want to run after installation.
E.g. to add Bukdu support:
```julia
using Pkg; pkg"add Bukdu"
using Bukdu
```


* the original code from https://github.com/pinx/heroku-buildpack-julia

[1]: https://julialang.org