# consult-latex-ref
Consult interface to LaTeX reference management. Bibliography management is already done wonderfully by `citar`. My other coding bits are here: https://github.com/sandyber/geekystuff.
# Sample configuration
```
(use-package consult-latex-ref
  :vc (consult-latex-ref :url "https://github.com/sandyber/consult-latex-ref" 
                 :rev :newest
                 :branch "main"
                 )
  :config
  (consult-customize consult-latex-toc :preview-key 'any)
  (setq consult-latex-ref-prompt-for-command t)
  (setq consult-latex-ref-label-command-alist
        '(("eq:" . "eqref")))
  (setq consult-latex-ref-commands
      '("ref" "eqref" "pageref"))
)
```
