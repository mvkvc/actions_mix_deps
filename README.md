# actions_mix_deps

This action installs and caches dependencies for Elixir projects using `mix deps.get` for faster subsequent runs.

## Usage

To include this action in your workflow, add the following line:

```yaml
- uses: actions_mix_deps@v1.0.1-alpha
  with:
    - erlang-version:
    - elixir-version:
    ...
```

The full list of inputs are:

```yaml
inputs:
  erlang-version:
    description: Erlang version to use
    required: true
    type: string
  elixir-version:
    description: Elixir version to use
    required: true
    type: string
  path:
    description: Path to the Mix project
    required: false
    type: string
    default: .
```
