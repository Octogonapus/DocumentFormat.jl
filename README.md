# DocumentFormat

[![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
[![Build Status](https://travis-ci.org/julia-vscode/DocumentFormat.jl.svg?branch=master)](https://travis-ci.org/julia-vscode/DocumentFormat.jl)
[![codecov.io](http://codecov.io/github/julia-vscode/DocumentFormat.jl/coverage.svg?branch=master)](http://codecov.io/github/julia-vscode/DocumentFormat.jl?branch=master)

An auto formatter for Julia.

## Overview

The main function to format code is `format`. When called with a string argument, that string is assumed to be code and a new string in which the code is formatted is returned. When called with an `AbstractPath` that points to a file, that file is being formatted. If called with an `AbstractPath` that points to a folder, all `*.jl` files in that folder are formatted.

The function `isformatted` checks whether a piece of code is formatted. It can be called with a string (assumed to hold code) or an `AbstractPath`.
