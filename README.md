program that allows you to draw simple graphs in the terminal and export them to files, there isnt much to add 

before compilation you need to have out/ and src/ directory and move .cpp and .h files to src/
then execute: make program

usage:

COMMAND LINE OPTIONS:
    -h --help     prints this help
    -w --write    specifies file to write

IN PROGRAM CONTROL:
    arrows - move cursor and choosed part (if any)
    F1     - selects part (first searches for box, then for line then for text in cursor pos)
                 box and text is selected by top left corner while line is selected wherever its points are
    F2     - unselects part
    F3     - removes selected part
    F4     - create box
    F5     - create line
    F6     - create text
    F7     - add point to a line and switch to it
    F8     - remove point from a line
    Q      - exits program
    w      - writes graph to "graph.txt" or file specified by user (for safety reasons, it should be empty file)
                 to be more specific it writes whatever is in 200x by 100y rectangle
    [ ]    - change box size on y axis
    { }    - change box size on x axis

    if text is selected you can type normally to add characters and remove them using backspace
        keep in mind that cursor is not changing its position when you are typing