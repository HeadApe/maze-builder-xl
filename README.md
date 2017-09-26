# maze-builder-xl
Maze Builder is an editor for game boards


Scope: creates and saves a top-down, 2d maze or architectural space of interconnected rooms or locations in a specialized binary format which can




Components and InForm methods

A. Rooms and paths
  1. picture boxes load a room graphic and a rotated path graphic, and display those in a grid (or on the form as the case with connections, ie paths)

B. Overall area that's expanded with track bars
  1. Zoom-able view when area exceeds screen size
  2. Simple scroll functionality, and/or a mini-map displaying in standard zoom
  3. columns or rows of area contract when not containing a room

C. Mouse used to paint rooms, or paths connecting rooms
  1 dragging within their space will change a room's offset
  2 standard offset values may be set
  3 RMB cancels a path or deletes a room (and attached connections)
  4 besides painting rooms, rows and columns can be inserted

D. Rooms can be drag-dropped about the grid, or offset
  1. dropping a room in an empty space = standard behavior
  2. dropping a room in place of another room
  0.0 Multiple rooms in selection

E. Connections take the appearance of paths
  1 connect one room visually with another
  2 can be of several user set types
  3 may be merged with existing connections to create a hybrid path

F. Rooms can be marked with a unique string to demark a special instance and such

G. Conveniences
preview mode : move a sprite through the area
kbd reassign menu
menu to provide paged printable sized png output files
undo: each operation creates a old state component as well as normal changes


**save file will contain

size of header : Map header and extra information
size of room data : room locations
size of path data : connection details
size of offset data : the offsets of rooms
size of custom value data, e.g. customized stats for a room
