---
layout: default
title: Japanese input on the command line (framebuffer)
comments: ""
disqus-id:
math: ""
---

## Upshot

- `uim-fep` seems to be the best option, on Bash.
- Using Emacs is quite possibly the best way overall, even if you’re a hardcore Vim user (like me)

### Things to add (it has been a while...):

- Something about how `Ctrl`-`i` or `Ctrl`-`o` was eaten up by Bash (since it got confused with the tab character?), so that one couldn’t set those to use as the shorten/lengthen keys.
- Where to place the config files?
- Graphical Emacs has a setup wizard which produces its own config files (even for Japanese input); what did I do with those?

## uim-fep

(at the moment I forgot where I was supposed to place this...)

{% highlight scheme %}
;; -*- mode: scheme -*-

(define-key generic-on-key? '("<Control>\\" "<Control>o"))
(define-key generic-off-key? '("<Control>\\" "<Control>o"))
(define-key anthy-on-key? 'generic-on-key?)
(define-key anthy-latin-key? 'generic-off-key?)
(define-key generic-cancel-key? "<Control>g")

(define-key generic-shrink-key? '("<IgnoreCase><Control>i" "<Shift>left"))
(define-key anthy-shrink-segment-key? 'generic-shrink-key?)

;; (define-custom 'anthy-extend-segment-key '("<IgnoreCase><Control>o" "<Shift>right")
;;                '(anthy-keys1)
;; 	       '(key)
;; 	       (N_ "[Anthy] extend segment")
;; 	       (N_ "long description will be here"))

;(define-key anthy-shrink-segment-key "<IgnoreCase><Control>i")


;; (define-key anthy-latin-key? '("<Control><Space>" generic-off-key?))
;; (define-key anthy-latin-key? '("<Control><Space>" generic-off-key?))
;; (define-key switch-im-key '())

;;(define-custom 'generic-on-key '("zenkaku-hankaku" "<Control> "))
;;(define-custom 'generic-off-key '("zenkaku-hankaku" "<Control> "))
{% endhighlight %}


## Emacs

I have the following in my `~/.emacs`.

{% highlight lisp %}
(set-fontset-font "fontset-default"
          'japanese-jisx0208
          '("IPAexGothic" . "iso10646-1"))
(prefer-coding-system 'utf-8)

;; This speeds up input?
(if (>= emacs-major-version 23)
    (setq anthy-accept-timeout 1))
{% endhighlight %}
