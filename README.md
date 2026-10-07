# AutomationWithPyautogui

Introduction to desktop automation with `pandas` and `pyautogui`: enters a list of names and e-mails, one by one, in a web system.

## The problem

More than 300 people had to be added to a web system. Doing it by hand means clicking the same buttons over and over while copying and pasting names and e-mails from a spreadsheet. The notebook does this loop on its own.

## How it works

1. Reads an Excel list with pandas (`Nome` and `Email` columns).
2. For each row (`iterrows`): clicks the button to add a person, clicks the name field, types the name, presses Tab, types the e-mail and clicks save, with short waits in between.

## Files

- `AutomatizacaoCurso.ipynb`: the notebook.
- `teste _ lista.xlsx`: a small sample list. The original list was replaced to avoid exposing real names and e-mails.

## Requirements

Python 3 with `pandas`, `openpyxl` and `pyautogui`.

## How to run

1. Open the target form and use `pyautogui.position()` to find the coordinates of each field and button.
2. Replace the coordinates in the loop with yours.
3. Run the cells. Do not touch the mouse while it runs.

## Notes

- Coordinates were recorded on the author's own monitor setup, so they must be replaced.
- A practice project. For a real task with a web page, a browser automation tool such as Selenium is usually more reliable than clicking screen positions.
