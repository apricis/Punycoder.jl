# Punycoder.jl
The implementation of Punycode converter in Julia. The conversion occurs as declared in [RFC 3492] (https://tools.ietf.org/html/rfc3492).

As Punycoder is not a package for now the interaction with the module can be done as follows:
```julia
julia> include("punycoder.jl")
Punycoder

julia> Punycoder.encode("bücher")
"bcher-kva"

julia> Punycoder.decode("bcher-kva")
"bücher"
```
