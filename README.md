# Personal Wardrobe Organizer

## Overview
The Personal Wardrobe Organizer is a Python-based application that helps users manage their wardrobe efficiently. It allows adding, viewing, updating, and deleting clothing items, and can also suggest random outfits. All items are stored in both a text file and an SQLite database.

## Features
- Add, update, view, and delete clothing items.
- Store data in both a text file (`wardrobe.txt`) and an SQLite database (`wardrobe.db`).
- Suggest random outfits from predefined combinations.
- Menu-driven interface.
- Input validation for English letters in clothing names and categories.

## Technologies Used
- Python 3.x
- SQLite (using Python's built-in `sqlite3`)
- File handling
- Random module

## Requirements
- Python 3.x
- No external libraries are needed (uses built-in modules only).

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Remas2Ahmad/wardrobe.git
   cd wardrobe-organizer
   ```

2. **Run the Application**:
   To start the program, run the Python script:
   ```bash
   python wardrobe.py
   ```
   This will create an SQLite database (`wardrobe.db`) and a text file (`wardrobe.txt`) if they do not already exist.

## Usage

1. Upon running the script, you will be presented with a menu with the following options:
   - 1. Add Clothing
   - 2. View Clothes
   - 3. Update Clothing
   - 4. Delete Clothing
   - 5. Suggest Outfit
   - 6. Exit

2. **Add Clothing**: Enter the name and category of the clothing item, and it will be added to both the database and the text file.

3. **View Clothes**: View all clothing items stored in the database with their name and category.

4. **Update Clothing**: Input the item ID, then the new name and category. The update will be reflected in both the database and the text.

5. **Delete Clothing**: Input the item ID to delete it. The change will be reflected in both the database and the text file.

6. **Suggest Outfit**: The program will randomly suggest an outfit, e.g., "Sweater with Leggings and Boots.

## File Structure
- `wardrobe.txt`: A plain text file that stores clothing items in a simple format (e.g., `Shirt (Top)`).
- `wardrobe.db`: An SQLite database file that contains a `clothes` table with columns: `id`, `name`, and `category`.

## Example Output

```bash
Wardrobe Management System
1. Add Clothing
2. View Clothes
3. Update Clothing
4. Delete Clothing
5. Suggest Outfit
6. Exit
Choose an option: 1
Enter clothing name: Shirt
Enter clothing category: Top
Clothing added successfully.
```

### Sample Outfit Suggestion:

```bash
Suggested outfit: Sweater with Leggings and Boots
```

