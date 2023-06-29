![alt text](https://files.catbox.moe/n7dlu3.png)

# nawanomicon
An org-roam for technical-scientific Stable Diffusion information.  

Terminal:
```
cd ~/org/roam
git clone https://github.com/tekakutli/nawanomicon
```
config.el
```
(setq org-roam-capture-templates
      '(
        ("n" "default" plain
         "%?"
         :if-new (file+head "%<%Y%m%d%H%M%S>-${slug}.org" "#+title: ${title}\n")
         :unnarrowed t)
        ("s" "stable diffusion" plain
         "%?"
         :if-new (file+head "nawanomicon/nodes/%<%Y%m%d%H%M%S>-${slug}.org" "#+title: ${title}\n#+filetags: :nawanomicon:\n")
         :unnarrowed t)
        )
)
```
