# Codebase to String

A tool to turn a codebase into a string for pasting into chatgpt. Currently, only Python and TypeScript are supported.

## Usage

1) Clone the repository: git clone https://github.com/alexpaden/codebase-to-string.git
2) Change directory: cd codebase-to-string
3) Run the Python script: python codebase_to_string.py
4) Run the TypeScript script: ts-node codebase_to_string.ts
5) The output will be saved in full_code.txt.

## How it Works

The script searches the current directory and its subdirectories for files with the specified file extension, excluding the script itself. It reads the contents of each file and concatenates them into a string. The resulting string is saved to a text file.

# Example Output
## Python
''' ./module_a.py '''
def function_a():
pass

''' ./module_b.py '''
def function_b():
pass

''' ./module_c.py '''
def function_c():
pass

''' ./main.py '''
from module_a import function_a
from module_b import function_b
from module_c import function_c

if name == 'main':
function_a()
function_b()
function_c()

## TypeScript
''' ./module-a.ts '''
export function functionA(): void {
return;
}

''' ./module-b.ts '''
export function functionB(): void {
return;
}

''' ./module-c.ts '''
export function functionC(): void {
return;
}

''' ./main.ts '''
import { functionA } from "./module-a";
import { functionB } from "./module-b";
import { functionC } from "./module-c";

functionA();
functionB();
functionC();
    
## Contributing

Feel free to submit pull requests or open issues for bug fixes, new features, or enhancements.
