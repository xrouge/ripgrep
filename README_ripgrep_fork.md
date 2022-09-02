This fork of ripgrep is located at: https://github.com/xrouge/ripgrep

There is a single difference compared to the main version:
add `vsgrep` switch in order to output the results in Visual Studio friendly format. This is similar to the `vimgrep` supported switch.
`vsgrep` format is useful if `rg` is called from within VS, directing the output to VS Output window.
In this case, clicking on a line would open the file in VS Editor.

Example:

	target\release\rg --vsgrep vsgrep crates\
 
 compare to:

	target\release\rg --vimgrep vsgrep crates\

The fork was necessary because [burntsushi rejected the suggestion](https://github.com/BurntSushi/ripgrep/discussions/1994)
to add support for VS output format to the main program, replying:
*Tools like Visual Studio should consider adapting to the grep format convention that has existed for decades.*
