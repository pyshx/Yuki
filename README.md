# Yuki
Yuki is a context-free grammar, lexer and predictive recursive descent parser for a C-like language in Go.

## Dependencies

- [gographviz](https://github.com/awalterschulze/gographviz), to generate the DOT specification
- [Graphviz](https://www.graphviz.org/), to generate the image from the DOT specification

## Usage

Please run `$ go run . [file]` where `[file]` represents an optional argument (which defaults to `test.txt`) to parse the file. If the parser accepts the program, it will generate a DOT specification of the parse tree depicting the leftmost derivation in `out.dot`. This specification can be run through Graphviz to generate the parse tree. We recommend doing `$ dot -Tpng -Gdpi=300 out.dot -o out.png`. 

## Lexer Testing
Input files for our lexer's test suite can be found in `src/tests/`. Please do `go test` to run the tests.

## References
- [Writing An Interpreter in Go by Thorsten Ball](https://interpreterbook.com/)
