# Julia v1.3.0 buildpack for Heroku

This is a Heroku buildpack for adding a [Julia binary][1] to your environment.

## Version

* Julia: `v1.3.0`

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

## Examples
 * https://github.com/wookay/starter-snake-julia


----

* the original code of heroku buildpack takes from https://github.com/pinx/heroku-buildpack-julia

[1]: https://julialang.org
