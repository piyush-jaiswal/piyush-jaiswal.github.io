---
layout: page
title: PDFConverse
description: Chat with your PDF! 
img: assets/img/pdfconverse/PDFConverse_demo.png
importance: 3
github: https://github.com/piyush-jaiswal/PDFConverse
width2: true
---

Upload your PDF and talk to it in natural language to gain insights and knowledge, just as you would talk to an LLM such as ChatGPT or Bard.

<div style="margin-top: 6%;"></div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pdfconverse/PDFConverse_diagram.png" title="PDFConverse" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b><i>How it works</i></b>
</div>

- PDF is divided up into small chunks
- Chunks are embedded using an embedding model
- Embeddings are stored in a vector store
- User asks a question
- Question is embedded using the same embedding model
- Similarity search of the embedded question is performed with docs in the vector store
- Question + similar docs are sent to LLM
- LLM answers the question, which is shown to the user

<div style="margin-top: 6%;"></div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pdfconverse/PDFConverse_demo.png" title="PDFConverse Demo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b><i>Demo</i></b>
</div>

<div style="margin-top: 4%;">
    <b>Project:</b> <a target="_blank" href="https://github.com/piyush-jaiswal/PDFConverse">https://github.com/piyush-jaiswal/PDFConverse</a>
</div>
