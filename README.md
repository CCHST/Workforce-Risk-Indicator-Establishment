# Workforce-Risk-Indicator-Establishment

## Overview

This repository contains code to calculate a labor risk indicator from text files using natural language processing techniques. The process involves analyzing text data to identify labor-related terms and their proximity to specified synonyms, thereby assessing the potential risk indicated by the text content.

## Contents

Approach 01. The code uses spaCy to process the tokens and identify the positions of any synonyms. It then counts the labor-related words that appear within 10 words of any synonym, and calculates the labor risk indicator as the ratio of matched labor words to the total word count in the file.

Approach 02. Based on Deloitte's labor-related keywords, vectorize the original labor_list_words and calculate cosine similarity, categorizing them into highly relevant (score 5) and generally relevant (score 3).