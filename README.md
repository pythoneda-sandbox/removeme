# pythoneda-sandbox/removeme

test domain

## How to declare it in your flake

python ~/github/pythoneda/pythoneda-tools-artifact/new-domain/pythoneda/tools/artifact/new_domain/application/new_domain_app.py -o pythoneda-shared-python -n shell -t "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" -g "D8DF2D915F27510072DFF42160856541692CA3C3" -p pythoneda.shared.shellox.removeme -d 'shared domain for shell operations'
Check the latest tag of the definition repository: https://github.com/pythoneda-sandbox-def/removeme, and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-sandbox-removeme = {
      [optional follows]
      url =
        "github:pythoneda-sandbox-def/removeme/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [https://nixos/nixpkgs](nixpkgs "nixpkgs") and [https://github.com/numtide/flake-utils](flake-utils "flake-utils").

The Nix flake is managed by the [https://github.com/pythoneda-sandbox-def/removeme](removeme "removeme") definition repository.

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-sandbox-removeme-python38`
- `#packages.[system].pythoneda-sandbox-removeme-python39`
- `#packages.[system].pythoneda-sandbox-removeme-python310`
- `#packages.[system].pythoneda-sandbox-removeme-python311`
