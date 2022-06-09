# solargraph-zeitwork-script
A script to generate namespaces to make solargraph work with zeitwork.

See this issue: https://github.com/castwide/vscode-solargraph/issues/200

It traverses folders in the project and generates namespaces from the folders, which is then deposited into a `namespaces.rb` file for solargraph to scan.

## How to Use
1. Copy `Makefile.local` and the `vscode-solargraph` folder into a rails project using zeitwork loader. Add `vscode-solargraph` and `Makefile.local` to your `.gitignore`.

2. edit Makefile.local to include the paths you'd like to scan.

3. run `make solargraph`.
