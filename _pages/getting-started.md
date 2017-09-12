---
layout: article
title:  "Getting Started"
excerpt: "Make your first API call with this quick start guide."
tags: [app-dev-getting-started]
show_related: true
author: steph_kim
---
## Header
paragraph

<div class="nav nav-tabs sub-nav app-nav gs__nav">
  <a href="#gs--install" class="active" data-toggle="tab" role="tab">
    <span class="gs__nav--icon">1</span>
    <span>Install</span>
  </a>
  <a href="#gs--auth" data-toggle="tab" role="tab">
    <span class="gs__nav--icon">2</span>
    <span>Auth</span>
  </a>
  <a href="#gs--run" data-toggle="tab" role="tab">
    <span class="gs__nav--icon">3</span>
    <span>Run</span>
  </a>
  <a href="#gs--upload" data-toggle="tab" role="tab">
    <span class="gs__nav--icon">4</span>
    <span>Upload</span>
  </a>
  <a href="#gs--data" data-toggle="tab" role="tab">
    <span class="gs__nav--icon">5</span>
    <span>Data</span>
  </a>
  <a href="#gs--data-analysis" data-toggle="tab" role="tab">
    <span class="gs__nav--icon">6</span>
    <span>Data Analysis</span>
  </a>
  <a href="#gs--done" data-toggle="tab" role="tab">
    <span class="gs__nav--icon">7</span>
    <span>Done!</span>
  </a>
</div>

<div class="tab-content">
  <section class="tab-pane active" id="gs--install" role="tabpanel">
    <p class="text-gray">instructions Hereeee: To get started you’ll need to install the Command Line Interface (CLI) on your local machine.</p>
    <div class="text-right"><a class="btn btn-xs">copy code</a></div>
    <pre class="gs__code"><code class="hljs">COMMAND HEREEEE: curl -sSf https://raw.githubusercontent.com/algorithmiaio/algorithmia-cli/master/install.sh | sh</code></pre>
    <p><b>Usage:</b> Copy and run this curl request in your Terminal.</p>
  </section>
</div>

<div class="tab-content">
  <section class="tab-pane" id="gs--auth" role="tabpanel">
    <!-- TODO: If not signed up prompt user to signup to get key -->
    <p class="text-gray">Authorize with your default API key</p>
    <div class="text-right"><a class="btn btn-xs">copy code</a></div>
    <pre class="gs__code"><code class="hljs">algo auth --key simx3V5DJFHU387JNMNK99</code></pre>
    <p><b>Usage:</b> Copy and run this curl request in your Terminal.</p>
  </section>
</div>

<div class="tab-content">
  <section class="tab-pane" id="gs--run" role="tabpanel">
    <p class="text-gray">Make your first API call to the Social Sentiment Analysis algorithm.</p>
    <div class="text-right"><a class="btn btn-xs">copy code</a></div>
    <pre class="gs__code"><code class="hljs">algo run algo://nlp/SocialSentimentAnalysis/0.1.4 -d '{
  "sentence": “Hello World! Today is a beautiful day!”
}'</code></pre>
    <p><b>Usage:</b> Copy and run this curl request in your Terminal.</p>
  </section>
</div>

<div class="tab-content">
  <section class="tab-pane" id="gs--upload" role="tabpanel">
    <p class="text-gray">Add data to your data portal</p>
    <div class="text-right"><a class="btn btn-xs">copy code</a></div>
    <pre class="gs__code"><code class="hljs">algo demo data</code></pre>
    <p><b>Usage:</b> Copy and run this curl request in your Terminal.</p>
  </section>
</div>

<div class="tab-content">
  <section class="tab-pane" id="gs--data" role="tabpanel">
    <p class="text-gray">View your data on Algorithmia</p>
    <div class="text-right"><a class="btn btn-xs">copy code</a></div>
    <pre class="gs__code"><code class="hljs">open https://algorithmia.com/data/hosted</code></pre>
    <p><b>Usage:</b> Copy and run this curl request in your Terminal.</p>
  </section>
</div>

<div class="tab-content">
  <section class="tab-pane" id="gs--data-analysis" role="tabpanel">
    <p class="text-gray">Analyze your newly added data</p>
    <div class="text-right"><a class="btn btn-xs">copy code</a></div>
    <pre class="gs__code"><code class="hljs">algo run algo://docs/AnalyzePDF/0.2.17 -d '["https://algorithmia.com/algorithms/weka/DigitRecognition","weka"]'</code></pre>
    <p><b>Usage:</b> Copy and run this curl request in your Terminal.</p>
  </section>
</div>

<div class="tab-content">
  <section class="tab-pane" id="gs--done" role="tabpanel">
    <p class="text-gray">Install in your language of choice</p>
    <div class="row lang-tile-container">
      {% assign sorted_clients = site.pages | where: "categories", "clients" | sort:"title" %}
      {% for post in sorted_clients %}
        {% include post-grid.html %}
      {% endfor %}
    </div>
  </section>
</div>

<div class="text-right m-T-l">
  <a href="">Need help?</a>
</div>