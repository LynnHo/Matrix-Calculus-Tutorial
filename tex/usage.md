```bash
# install latex
sudo apt install texlive-full dvisvgm

# install readme2tex
conda create -n readme2tex python=3
source activate readme2tex
pip install readme2tex

# generate README.md and examples.md
python -m readme2tex --nocdn --output "README.md" --svgdir svg  "tex/README.tex.md"
python -m readme2tex --nocdn --output "examples.md" --svgdir svg  "tex/examples.tex.md"
```
