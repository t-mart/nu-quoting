# Nushell Quoting Issue

## Reproduction

1. Ensure you have `node` and `npm` installed.
2. Run a non-exhibiting example:

   ```shell
   npm run repro a b c
   # Outputs like:
   # [
   #   'C:\\Users\\tim\\scoop\\apps\\nodejs\\18.7.0\\node.exe',
   #   'C:\\Users\\tim\\code\\nu-quoting\\index.js',
   #   'a',
   #   'b',
   #   'c'
   # ]
   ```

   Run the exhibiting example:

   ```shell
   npm run repro "a b c"
   # Outputs like:
   # [
   #   'C:\\Users\\tim\\scoop\\apps\\nodejs\\18.7.0\\node.exe',
   #   'C:\\Users\\tim\\code\\nu-quoting\\index.js',
   #   '"a b c"'
   # ]
   ```

   **Note the quoting of the abc argument.**
