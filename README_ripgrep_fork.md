This fork of ripgrep is located at: https://github.com/xrouge/ripgrep
There is a single difference compared to the main version : add 'vsgrep' switch to output the results in Visual Studio friendly format.
This format is useful if rg is called from within VS, directing the output to VS Output window. In this case, clicking a line would open the file in VS Editor.
The fork was necessary because burntsushi rejected the suggestion to add VS output format to the main program, suggesting: "Tools like Visual Studio should consider adapting to the grep format convention that has existed for decades."
https://github.com/BurntSushi/ripgrep/discussions/1994