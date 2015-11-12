# rustfmt.el

[![MELPA][badge-melpa]](http://melpa.org/#/rustfmt)

Format rust code in emacs using [rustfmt][].

## Usage

Run <kbd>M-x rustfmt-format-buffer</kbd> to format the current buffer.

For convenience, you may bind it to a key, such as:
```el
(define-key rust-mode-map (kbd "C-c C-f") #'rustfmt-format-buffer)
```

Alternatively, run rustfmt before saving rust buffers:
```el
(add-hook 'rust-mode-hook #'rustfmt-enable-on-save)
```

[rustfmt]: https://github.com/nrc/rustfmt
[badge-melpa]: http://melpa.org/packages/rustfmt-badge.svg
