In E-Commerce, Keyword stuffing is a prevalent issue. On a daily basis, thousands of new products are added to the product catalog. 
To make these products accessible on the website, it becomes necessary to assign search keywords to these products. 
Following problems are involved in creating and curating these search keywords.
<ol >
  <li> Requires Manual effort. This activity needs to be performed by Cataloging team or the Sellers</li>
  <li> Room for spell errors. Misspelt keywords might not match with the search keys that customers enter</li>
  <li> Keyword Stuffing : When the sellers use irrelevant keywords popular on the platform to push their product</li>
</ol>

Since LLMs are good for language generation uses-cases, we attempted to use an LLM to generate search keywords.
In this approach, we leverage mistralai/Mistral-7B-Instruct-v0.2 model which is an instruction fine-tuned LLM
It has a context window of 32K characters, which makes it suitable for this task, as large amount of text neeeds to be sifted through to generate keywords.

Due to operational infrastructure constraints, the LLM was quantized using BitsAndBytes quantization to run in 4 bit
It required 5GB to load and inference on Google Colab T4 GPU


