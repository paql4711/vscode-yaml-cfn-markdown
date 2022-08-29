# Change Log
## [2.0.2]
- Bugs
    - !Sub | will not allow comment in the same line
    - Type Class highlighting was also highlighting other Types like Domain Records
    - IAM Actions not closed with " or ' were not highlighted, so issues could not be easily found
    - Variable Names can now contain -
    - All functions except !Sub can now be used with { }, !Sub will still require quotes to not break the syntax
    - Default scope for code injections was set to have highlighting of default objects correct. 
## [2.0.1]
- Initial release
