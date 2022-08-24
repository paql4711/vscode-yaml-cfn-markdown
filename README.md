# VSCode YAML Grammar Injection for AWS Cloudformation support 
[![Version](https://img.shields.io/visual-studio-marketplace/v/paql4711.aws-cloudformation-yaml-highlighter.svg?style=flat)](https://marketplace.visualstudio.com/items?itemName=paql4711.aws-cloudformation-yaml-highlighter)
[![Version](https://img.shields.io/visual-studio-marketplace/d/paql4711.aws-cloudformation-yaml-highlighter.svg?style=flat)](https://marketplace.visualstudio.com/items?itemName=paql4711.aws-cloudformation-yaml-highlighter)

AWS Cloudformation relies on YAML with the addition of several functions, inline codes and variables.
These are only partially highlighted within the default YAML markup, so the extension will support highlighting relevant parts of the code.

## Examples
### YAML Cloudformation  Highlighting:
![features](/images/YAML_CFN_Highlight.png)

### Using Inline Code:
![features](/images/YAML_Inline_Code.png)



## Usage
The extension is ready to use after the installation for Syntax highlighting.

To enable inline code formatting the start and end Tag needs to be set as comment since Cloudformation has no pattern to identify start / end of certain langugaes.

The formatting will only work behind | with exactly the defined Syntax.
```YAML
E.g.:
Code: !Sub | #.ps1 (Change .ps1 by Codelanguage fileextension)
      <Some Powershell Code>
      <Some Powershell Code>
      <Some Powershell Code>
```




## Supported Variables
Following variables are currently included in the auto-highlighting
- Functions starting with ! or Fn:: **(Fn:: is not fully supported yet!)**
    - e.g. !Ref, !Sub
- Variables within Sub Strings
    - e.g. !Sub "Hello from ${region}"
- Static variables for AWS:: Values
    - e.g. AWS::AccountId
- Resource Type will be highlighted as Class


## Supported Inline Codes

Following file extensions / codes are supported in the current version:
- PowerShell (.ps1)
- Python (.py)
- JSON (.json)
- TypeScript (.ts)
- Shellscript (.sh)
- JavaScript (.js)
- Java (.java)
- SQL (.sql)
- XML (.xml)
- HTML (.html)
- CSS (.css)

## Contribution
The entire project is open source and can be found on:
- https://github.com/paql4711/paql4711-vscode-yaml-cfn-markdown

In case you experience any issues please raise them directly within GitHub, for contributing please feel free to raise a pull request.