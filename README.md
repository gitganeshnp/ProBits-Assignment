<h1>Probits Technologies - Assignment</h1> <br>

<h2><i>Problem Statement :</i></h2> 
<p><b>Extract the E-mail ID and Technologies from a resume or profile which is in the format of docx</b></p>
<p>The text extraction from a docx requires different libraries, processes.</p>

<h3>Libraries Used</h3>
<ul>
 <li>import docxpy</li>
 <li>import re</li>
 <li>from docx import *</li>
 <li>import pandas as pd</li>
 <li>import os</li>
 <li>import numpy as np</li>
 <li>import pandas as pd</li>
 <li>import string</li>
 <li>import nltk</li>
 <li>from nltk.corpus import stopwords</li>
 <li>from itertools import chain</li></ul>

<p>To solve this problem I used two different approaches where I can get Email-Id and Skills, Technologies</p>

<h3><i>Approach</i></h3>

<ul>
  <li>Regular Expression for Email-ID extraction and simple raw python code for skills and technologies</li>
  <li>Used NLTK to extract skills and Technologies</li></ul>
  
<h3><b>Breif explanation of two approaches</b></h3>

<h4>Extracting Email-ID</h4>
<li>Processed the document using docxpy.process</li>
<li>Used re.findall() to extract email-id</li>

<h4>Extracting skills and technologies using raw python code</h4>
<li>After Processing the document, Making paragraphs using document.paragraphs</li>
<li>Using para.style.name == "Heading 1" to extract skills and technologies</li>

<h4>Extracting Skills and Technologies usnig NLTK</h4>
<li>Collected the finite skill set infromation from external resource</li>
<li>Converting all skills into lowercase and string of lists</li>
<li>Processing the resume document and retaining only alphabets and numbers by removing all punctuations and special characters</li>
<li>Next step I removed all stop words</li>
<li>Preparing Sentence and word tokens to create Unigram and Bigram words</li>
<li>creating Bigrams using nltk.bigrams</li>
<li>Iterating a loop with boolean conditions to match any skills are there in input resume document</li>
<li>Producing Output list and converting it to structured data</li>
<li>Writing the output file into disk</li>
<li>Tested with multiple resumes and getting skills and technologies properly</li>
