# flycheck-mix
Support Elixir mix in flycheck

This package adds support for Elixir mix to flycheck.
To use it, add to your init.el:

    (require 'flycheck-mix)
    (flycheck-mix-setup)

Elixir compilation uses macros and it can run arbitrary code.
You should use `elixir-mix` checker only with trusted projects.
To enable it for given project add directory local variable
`flycheck-mix-enable-checking` and set it to `t`
You can easily do it by running `M-x add-dir-local-variable`
then for mode specify `elixir-mode`
variable name `flycheck-mix-enable-checking`
and for value `t`
You can also enable it globally with

    (setq flycheck-mix-enable-checking t)

but this is not recommended.
