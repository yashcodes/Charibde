# CharibdeOptim

[![Stable](https://img.shields.io/badge/docs-stable-blue.svg)](https://yashcodes.github.io/CharibdeOptim.jl/stable)
[![Dev](https://img.shields.io/badge/docs-dev-blue.svg)](https://yashcodes.github.io/CharibdeOptim.jl/dev)
[![Build Status](https://travis-ci.com/yashcodes/CharibdeOptim.jl.svg?branch=master)](https://travis-ci.com/yashcodes/CharibdeOptim.jl)
[![Build Status](https://ci.appveyor.com/api/projects/status/github/yashcodes/CharibdeOptim.jl?svg=true)](https://ci.appveyor.com/project/yashcodes/CharibdeOptim-jl)
[![Codecov](https://codecov.io/gh/yashcodes/CharibdeOptim.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/yashcodes/CharibdeOptim.jl)
[![Coveralls](https://coveralls.io/repos/github/yashcodes/CharibdeOptim.jl/badge.svg?branch=master)](https://coveralls.io/github/yashcodes/CharibdeOptim.jl?branch=master)
[![Build Status](https://api.cirrus-ci.com/github/yashcodes/CharibdeOptim.jl.svg)](https://cirrus-ci.com/github/yashcodes/CharibdeOptim.jl)

This Julia package is for to solve mathematical optimisation problems of both unconstrained as well as constrained kind. The package uses the approach named *Charibde* in which it uses two algorithm *Differential Evolution* and *Interval Branch & Contract algorithm* to achieve solution which is quite fast to get and guaranteed correct in case of difficult problems than using just any one of the algorithm among them two.

The package makes these two algorithm run in parallel on two different processors (means: there should be atleast 2 workers present on that julia session) of the machine while being in contact (i.e share the best known solution with each other) with one another through remotechannels.

The package also allows us to use just *Interval Branch & Contract* algorithm to solve the problems rather than using Charibde.

The package can also be use through JuMP syntax.

## Documentation
Documentation for the package is available

## Author

- Yashvardhan Sharma, IIT Kharagpur, West Bengal, India

## Mentors

- [David P. Sanders](http://sistemas.fciencias.unam.mx/~dsanders),
Departamento de Física, Facultad de Ciencias, Universidad Nacional Autónoma de México (UNAM)

- [Charlie Vanaret](https://cvanaret.wordpress.com/)
Researcher at Fraunhofer ITWM

## References:
- [Charibde - Archive ouverte HAL](https://hal.archives-ouvertes.fr/hal-01168096/document)
- [DOCTORAT DE L'UNIVERSITÉ DE TOULOUSE](http://ethesis.inp-toulouse.fr/archive/00002966/01/vanaret.pdf)
