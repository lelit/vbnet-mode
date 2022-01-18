# vbnet-mode

A GNU/Emacs major mode to edit [`VB.NET`](https://en.wikipedia.org/wiki/Visual_Basic_.NET) source.

This is taken from [`VbDotNetMode`](https://www.emacswiki.org/emacs/VbDotNetMode) and improved
here and there to fulfill my needs.

## Installation

As I do not foresee releasing the package on [`MELPA`](https://melpa.org/), you must install
this manually, copying the `vbnet-mode.el` somewhere in your `load-path` and then activate it:

``` emacs-lisp
(autoload 'vbnet-mode "vbnet-mode" "Mode for editing VB.NET code." t)
(add-to-list 'auto-mode-alist '("\\.vb\\'" . vbnet-mode))
```

If you use [`Doom Emacs`](https://github.com/hlissner/doom-emacs) then something like the
following should work:

``` emacs-lisp
(package! vbnet-mode
  :recipe (:host github :repo "lelit/vbnet-mode"))

(use-package! vbnet-mode
  :mode "\\.vb\\'")
```
