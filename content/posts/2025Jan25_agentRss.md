+++
date = '2025-01-25T17:12:44-05:00'
draft = false
title = '2025Jan25_agentRss'
+++

## Use Hugging Face smolagents to grab RSS links from any journal

[Here's a python script](https://github.com/samesense/get-rss) to find the RSS url on any journal website. It leverages [smolagents](https://huggingface.co/docs/smolagents/en/index) and meta-llama/Llama-3.3-70B-Instruct. The journal’s HTML is grabbed with a custom smolagent tool powered by Playwright. Html parsing is handled by Beautiful Soup (bs4).  
