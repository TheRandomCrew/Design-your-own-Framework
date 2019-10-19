# Objetives

* make it responsive
* sections grids responsiveness
* images resize
* Set the breakpoints
* mobile first approach
* make a great README
* use github flow

* show a grid overlay
    + 10 columns
    + gutter
    + gap 10px

# Steps to follow

- [ ] Make grid utilities
- [ ] make mobile view
- [ ] Add Components to each sections
- [ ] Add tablet media queries
- [ ] make desktop queries
- [ ] Add nav change
- [ ] check for sticler errors

# Sections

* portrait blocks, grid, columns examples
    + Presentation 
    + index
    + columns
        - A button to show the columns overlay
    + Containers, rows, columns and grid use
        - container
        - rows
        - columns
    + Responsiveness
        - Auto Responsiveness
            4 columns on mobile, 10 on the rest
        - Set your columns by size
    + layout examples
        - Holy Grail
        - Card
        - navbar
        - Gallery

.row { # a lot of rows, use empty space
    display: flex;
    flex-wrap: wrap:

    &__col-5 {
        flex-basis: 50%;
    }
    &__col-2 {
        flex-basis: 20%;
    }

    &__col-sm-2{
        flex-basis: inherit;
        //media query{
            flex-basis: 20%
        }
    }
}