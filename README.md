# Unexpected Panic from Nil Map Access in Go

This repository demonstrates a common error in Go programming: attempting to access an element of a map before checking if the map is nil. This results in a runtime panic.

## The Bug

The `bug.go` file shows a simple function that attempts to assign a value to a map key without checking if the map is initialized.  If the map is nil, this will trigger a runtime panic.

## The Solution

The `bugSolution.go` file provides the corrected version.  It checks if the map is nil before accessing its elements, preventing the panic.

## How to reproduce

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `go run bug.go` to see the panic.
4. Run `go run bugSolution.go` to see the corrected version.