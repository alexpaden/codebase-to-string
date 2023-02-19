# Codebase to String

A tool to turn a codebase into a string for pasting into chatgpt. Currently, only Python is supported.

## Usage

1. Clone the repository: `git clone https://github.com/your-username/codebase-to-string.git`
2. Change directory: `cd codebase-to-string`
3. Run the script: `python codebase_to_string.py`
4. The output will be saved in `full_code.txt`.

## How it Works

The script searches the current directory and its subdirectories for Python files, excluding the script itself. It reads the contents of each file and concatenates them into a string. The resulting string is saved to a text file.

## Example Output

''' ./module_a.py '''
def function_a():
pass
'''

''' ./module_b.py '''
def function_b():
pass
'''

''' ./module_c.py '''
def function_c():
pass
'''

''' ./main.py '''
from module_a import function_a
from module_b import function_b
from module_c import function_c

if name == 'main':
function_a()
function_b()
function_c()
'''


## Contributing

Feel free to submit pull requests or open issues for bug fixes, new features, or enhancements.
