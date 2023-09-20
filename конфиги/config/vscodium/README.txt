СКАЧАЙТЕ VSCodium
НА ОСНОВЕ НЕГО СООБСТВЕННО ПОСТРОЕНО ВСЕ IDE

VSCodium

https://github.com/VSCodium/vscodium

Модули

https://marketplace.visualstudio.com/items?itemName=JerryHong.autofilename

https://marketplace.visualstudio.com/items?itemName=tdennis4496.cmantic

https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools // Версия 1.12.4

https://github.com/microsoft/vscode-cpptools/releases/tag/v1.12.4

https://marketplace.visualstudio.com/items?itemName=HungVo.htext

https://marketplace.visualstudio.com/items?itemName=FleeXo.cpp-class-creator

https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph

https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools
P.S.
В папку с файлами я не добавил cpptools, надо скачать самому под свою операционную систему файл vsix cpptools
https://github.com/microsoft/vscode-cpptools/releases/tag/v1.12.4
именно этой версии



settings.json

{
    "cmake.cmakePath": "c:\\Program Files\\CMake\\bin\\cmake.exe",
    "workbench.startupEditor": "none",
    "cmake.buildDirectory": "${workspaceFolder}/../build_${workspaceRootFolderName}-${buildType}",
    "editor.wordWrap": "on",
    "cmake.configureOnOpen": true,
    "cpp.creator.headerFileNamePreset": "{{*CLASSNAMELOWER*}}.h",
    "cpp.creator.sourceFileNamePreset": "{{*CLASSNAMELOWER*}}.cpp",
    "qttools.creator": "c:\\msys64\\mingw64\\bin\\qtcreator.exe",
    "git.enableSmartCommit": true,
    "[cpp]": {
        "editor.defaultFormatter": "ms-vscode.cpptools"
    },
    "C_Cpp.default.cppStandard": "c++17",
    "C_Cpp.default.cStandard": "c17",
    "C_Cpp.intelliSenseCacheSize": 10120,
    "C_Cpp.intelliSenseMemoryLimit": 6096,
    "C_Cpp.default.intelliSenseMode": "windows-gcc-x64",
    "C_Cpp.default.compilerPath": "d:\\\\mingw64\\\\bin\\\\g++.exe"
}

.clang-format

BasedOnStyle: Google
AccessModifierOffset: -4
ConstructorInitializerIndentWidth: 2
AlignEscapedNewlinesLeft: false
AlignTrailingComments: true
AllowAllParametersOfDeclarationOnNextLine: false
AllowShortIfStatementsOnASingleLine: false
AllowShortLoopsOnASingleLine: false
AllowShortFunctionsOnASingleLine: None
AlwaysBreakTemplateDeclarations: true
AlwaysBreakBeforeMultilineStrings: true
BreakBeforeBinaryOperators: false
BreakBeforeTernaryOperators: false
BreakConstructorInitializersBeforeComma: true
BinPackParameters: true
ColumnLimit: 500
ConstructorInitializerAllOnOneLineOrOnePerLine: true
DerivePointerBinding: false
PointerBindsToType: true
ExperimentalAutoDetectBinPacking: false
IndentCaseLabels: true
MaxEmptyLinesToKeep: 1
NamespaceIndentation: None
ObjCSpaceBeforeProtocolList: true
PenaltyBreakBeforeFirstCallParameter: 19
PenaltyBreakComment: 60
PenaltyBreakString: 1
PenaltyBreakFirstLessLess: 1000
PenaltyExcessCharacter: 1000
PenaltyReturnTypeOnItsOwnLine: 90
SpacesBeforeTrailingComments: 2
Cpp11BracedListStyle: false
Standard: Auto
IndentWidth: 4
TabWidth: 4
UseTab: Never
IndentFunctionDeclarationAfterType: false
SpacesInParentheses: false
SpacesInAngles: false
SpaceInEmptyParentheses: false
SpacesInCStyleCastParentheses: false
SpaceAfterControlStatementKeyword: true
SpaceBeforeAssignmentOperators: true
ContinuationIndentWidth: 4
SortIncludes: false
SpaceAfterCStyleCast: false

# Configure each individual brace in BraceWrapping
BreakBeforeBraces: Custom

# Control of individual brace wrapping cases
BraceWrapping: {
    AfterClass: 'true'
    AfterControlStatement: 'true'
    AfterEnum : 'true'
    AfterFunction : 'true'
    AfterNamespace : 'true'
    AfterStruct : 'true'
    AfterUnion : 'true'
    BeforeCatch : 'true'
    BeforeElse : 'true'
    IndentBraces : 'false'
}
