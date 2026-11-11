# Python Movie Manager

A command-line movie collection application developed for **Lab 3 of GIK29B: Python and R Programming** at Dalarna University, Sweden, during my Data Science master's studies.

The exercise demonstrates a class-based data model and create, read, update and delete (CRUD) operations through an interactive menu.

## Features

- Add a movie with a user-selected ID, title, genre and playing time.
- Reject duplicate IDs when adding a movie.
- Display all movies in a formatted table.
- Update the title, genre or playing time individually or together.
- Delete a movie by ID after confirmation.
- Check for non-empty text, positive integer IDs and durations, and valid menu selections.

## Getting started

Python 3 is required. No third-party packages are needed.

Download or clone the repository, open a terminal in its root folder, and run:

```bash
python movies.py
```

Use `python3 movies.py` if your system uses `python3` for Python 3.

## Example workflow

1. Choose **1** to add a movie. Enter ID `1`, title `Example Film`, genre `Drama` and playing time `95` minutes.
2. Choose **2** to display the collection.
3. Choose **3**, enter ID `1` and select which details to update.
4. Choose **4** and enter ID `1` to delete the record after confirmation.
5. Choose **5** to quit.

Movie IDs are entered by the user, not generated automatically. The update menu changes descriptive fields while retaining the existing ID.

## Design and storage

All implementation is in `movies.py`. The `Movie` class encapsulates its ID, title, genre and playing time through name-mangled attributes with getter and setter methods. Separate functions handle input validation, ID lookup, CRUD operations and the menu. Named constants identify the main menu choices.

The collection is stored in a list for the current session only. Each run starts empty, and records are discarded when the program exits. There is no file or database persistence.

The file is intended to be run as an interactive script. Its top-level `main()` call also starts the menu if the file is imported.

## Academic context

This repository presents the movie application separately for convenient browsing. The broader [Python programming course collection](https://github.com/iamalif/python-programming-msc/tree/main/python-lab3-assignment) includes the lab context and related assignment material.

## Skills demonstrated

Python classes, encapsulation, lists of objects, CRUD operations, input validation, function decomposition and command-line interaction.
