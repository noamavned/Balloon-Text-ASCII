# ASCII BALLOON

The `BALLOON` class in Python generates ASCII art representations of strings in a balloon style. Each letter and space has a predefined ASCII pattern.

## Class Overview

The `BALLOON` class includes predefined ASCII art for the following characters:
- Letters: A-Z
- Space

## Functions

### `__init__(self)`

Initializes the class with ASCII patterns for each supported character.

### `__get_letter__(self, char)`

- **Input**: A character `char`.
- **Output**: The corresponding ASCII art pattern as a list of strings.
- **Description**: Retrieves the ASCII pattern for the given character. Returns a pattern of empty spaces if the character is not found.

### `__generate_letter_grid__(self, s)`

- **Input**: A string `s`.
- **Output**: A list of ASCII art patterns for each character in the string.
- **Description**: Converts each character in the input string into its corresponding ASCII art pattern.

### `__combine_rows__(self, letter_grids)`

- **Input**: A list of ASCII art patterns `letter_grids`.
- **Output**: A list of strings where each string represents a row of combined ASCII art patterns.
- **Description**: Combines the rows of multiple ASCII art patterns into a single list of strings.

### `create_ascii_balloon(self, s)`

- **Input**: A string `s`.
- **Output**: A single string representing the combined ASCII art for the entire input string.
- **Description**: Generates the complete ASCII art for the input string by combining the patterns of individual characters.

## Example Usage

```python
balloon = BALLOON()
ascii_art = balloon.create_ascii_balloon("HELLO")
print(ascii_art)


