# Dependencies
python 3.11
!pip install cohere

# Setup
Jupyter script should be operated within its own working directory.
Directory should include a file with the api key for the program to read, this file should be named within the second cell of the script.
Directory should also include a folder named saved, but this will be created on the first execution so you needn't worry about this.

# Usage
User will be asked to input a prompt for the text they would like generated,
they then will be asked if they would like to tweak any of the default parameters.

Application prompts are color coded in response to the action the user should take:
- Blue messages are for guidance,
- Yellow messages are for instruction,
- Red messages are for attentive action,
- Green messages are for successful actions

The program uses some input validity features for easier usage:
- Color coded responses that allow for easier reading of the interface.
- Inputs are pared down to more universal forms, space and case-sensitivity issues are mitigated.
- Order of parameters specified is not important.
- Users are informed of the exact parameter that is invalid at the moment it is parsed.
- Program accounts for invalid keys, value types, and even defining the same parameter twice.
- Program loops indefinitely until user chooses to exit.
- Program offers two chances to save, once when text is generated and again when exited should the
user have opted out of the first chance.
- File names specified by the user are denied any special character input and do so without
interrupting the program.
