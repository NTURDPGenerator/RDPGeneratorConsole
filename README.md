# RDPGeneratorConsole
An Recursive Descent Parser (RDP) Code Generator created for students of NTU CZ3007.

# Introduction
The RDP Generator application produces Recursive Descent Parser (RDP) code based on an input Context-Free Grammar (CFG).

It takes in a text file containing the specification of the CFG, and outputs RDP code written in various languages (C++, Java, and C#). Note that you can choose which languages to generate.

The application can also generate detailed reports together with the RDP code, that explain the functions of the RDP. You can choose to enable or disable this feature when using the application.

# Usage Instructions
1. Download the program files to your device (either via ZIP or cloning the repository).
2. Create two folders, "config" and "logs", in the folder containing the downloaded files.
3. Create a text file and write your CFG here. You can store this text file anywhere on your device.
4. Open a Command Prompt and navigate to the folder containing the downloaded files.
5. Enter "RDPGeneratorConsole [path to CFG file]".
6. Follow the instructions on the Command Prompt.
7. If the RDP code is successfully generated, you should see new folders (e.g. "output-cpp", "output-cs", "output-java") appear in the folder. These folders contain the RDP code, as well as the generated reports (if Report Generation is enabled).
8. If the CFG contains any errors, an error message will be shown on the Command Prompt.
  
# CFG Formatting Guidelines
1. The Non-Terminal on the Left of the First Rule is the Start Terminal.
2. The arrow '->' is used to separate the LHS and RHS of a Production Rule.
3. Production Rules belonging to a Non-Terminal can be separated by the OR '|' symbol, or by new lines. For example :
  
   A -> a | b
  
   and
  
   A -> a
   
   A -> b
  
   are both equally valid.
  
4. An Epsilon-only Production Rule is indicated by an empty Rule.
  
# Important Notes
1. Please ensure all program files (downloaded from this repository) are kept in the same directory.
2. Reports are generated in the form of inline Doxygen documentation in the RDP code.
  
   If Report Generation is enabled, a file called "doxyfile.ini" will be generated together with the RDP code.
  
   To view the report, open a Command Prompt, navigate to the folder containing doxyfile.ini, and enter "doxygen doxyfile.ini".
  
   This will produce a html folder, which contains HTML files containing the documentation. You can open these files in a browser.
  
   Note that this requires Doxygen to be installed on your device. Please visit https://www.doxygen.nl/download.html to download Doxygen.
