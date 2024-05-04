## Stat 114 Final Project Vignette - GPT Integration for Biomedical PDF Summaries

The objective of this project is to automatically summarize sections of biomedical research papers as dictated by user highlights. Within this tutorial, you can use our tools to automatically create a Beamer slideshow that summarizes sections of Love et al's DESeq2 paper:

1. Clone this repo with
```sh
git clone git@github.com:MattKotzbauer/pdf-reader-vignette.git 
```
2. Mark down `love.pdf` by highlighting the starting and ending sentences of sections you would like summarized. For each pair of highlights, our program will end up summarizing the text between them. Any PDF-reading software should work for annotating the document, a few examples being
- Adobe Acrobat
- Microsoft Edge
- Preview
- Okular

3. Call our Python script to generate LLM prompts based on your annotations. In this case, we pass your annotated verison of `love.pdf` as an argument, telling our script to use the text and locations of its annotations to generate its prompts

```sh
python getTextPrompts.py love.pdf
```

The content of your prompts will then be saved to `text_prompts.txt`, with each 

4. call oru script to generate slideshow

5. compile the slideshow on overleaf, save to pdf, and boom u now have slideshow






